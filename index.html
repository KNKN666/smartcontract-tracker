import { useState, useEffect } from "react";
import { BarChart, Bar, XAxis, YAxis, Tooltip, ResponsiveContainer } from "recharts";

export default function SmartContractTracker() {
  const [contracts, setContracts] = useState([]);
  const [contractName, setContractName] = useState("");
  const [deadline, setDeadline] = useState("");
  const [reminder, setReminder] = useState("");
  const [email, setEmail] = useState("");
  const [status, setStatus] = useState("Pending");
  const [isAuthenticated, setIsAuthenticated] = useState(false);
  const [username, setUsername] = useState("");
  const [password, setPassword] = useState("");

  const addContract = () => {
    if (!contractName || !deadline || !reminder || !email) return;
    setContracts([...contracts, { name: contractName, deadline, reminder, email, status }]);
    setContractName("");
    setDeadline("");
    setReminder("");
    setEmail("");
    setStatus("Pending");
  };

  useEffect(() => {
    const today = new Date().toISOString().split("T")[0];
    contracts.forEach(contract => {
      if (contract.reminder === today) {
        alert(`Reminder: Your contract '${contract.name}' is due soon!`);
      }
    });
  }, [contracts]);

  const login = () => {
    if (username === "admin" && password === "password") {
      setIsAuthenticated(true);
    } else {
      alert("Invalid credentials");
    }
  };

  const contractData = [
    { status: "Pending", count: contracts.filter(c => c.status === "Pending").length },
    { status: "Active", count: contracts.filter(c => c.status === "Active").length },
    { status: "Expired", count: contracts.filter(c => c.status === "Expired").length }
  ];

  if (!isAuthenticated) {
    return (
      <div className="flex flex-col items-center justify-center h-screen">
        <h1 className="text-3xl font-bold mb-4">Login</h1>
        <input placeholder="Username" value={username} onChange={(e) => setUsername(e.target.value)} className="mb-2 p-2 border rounded" />
        <input type="password" placeholder="Password" value={password} onChange={(e) => setPassword(e.target.value)} className="mb-2 p-2 border rounded" />
        <button onClick={login} className="p-2 bg-blue-500 text-white rounded">Login</button>
      </div>
    );
  }

  return (
    <div className="p-10 w-full font-sans">
      <h1 className="text-3xl font-bold mb-6">SmartContract Tracker</h1>
      <div className="mb-4">
        <input placeholder="Contract Name" value={contractName} onChange={(e) => setContractName(e.target.value)} className="p-2 border rounded mr-2" />
        <input type="date" placeholder="Deadline" value={deadline} onChange={(e) => setDeadline(e.target.value)} className="p-2 border rounded mr-2" />
        <input type="date" placeholder="Reminder Date" value={reminder} onChange={(e) => setReminder(e.target.value)} className="p-2 border rounded mr-2" />
        <input type="email" placeholder="Email" value={email} onChange={(e) => setEmail(e.target.value)} className="p-2 border rounded mr-2" />
        <select value={status} onChange={(e) => setStatus(e.target.value)} className="p-2 border rounded">
          <option value="Pending">Pending</option>
          <option value="Active">Active</option>
          <option value="Expired">Expired</option>
        </select>
        <button onClick={addContract} className="p-2 bg-green-500 text-white rounded ml-2">Add Contract</button>
      </div>
      <ResponsiveContainer width="100%" height={300}>
        <BarChart data={contractData}>
          <XAxis dataKey="status" />
          <YAxis />
          <Tooltip />
          <Bar dataKey="count" fill="#82ca9d" />
        </BarChart>
      </ResponsiveContainer>
      <div className="mt-6 p-4 border-t">
        <h2 className="text-lg font-bold">Data Privacy Notice</h2>
        <p className="text-sm">
          This website complies with the Data Privacy Act of 2012 (Republic Act No. 10173) of the Philippines. We ensure that all collected contract data is kept secure and used solely for contract tracking purposes.
        </p>
      </div>
    </div>
  );
}
