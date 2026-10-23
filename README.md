# Survival-Rom-nia
import { useEffect, useState } from 'react';  export default function App() {   const [servers, setServers] = useState([]);   useEffect(() => {     fetch('http://localhost:3001/api/servers')       .then(res => res.json())       .then(data => setServers(data));   }, []);    return (     &lt;div>       &lt;h1>Romania Server&lt;/h1>       
