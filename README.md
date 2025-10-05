# stack-sprints
spints and stack dev
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Moment Connect - Development Roadmap</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            box-sizing: border-box;
        }
        .sprint-card {
            transition: all 0.3s ease-in-out;
        }
        .sprint-card:hover {
            transform: translateY(-4px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        .tech-badge {
            transition: all 0.2s ease-in-out;
        }
        .tech-badge:hover {
            transform: scale(1.05);
        }
        .timeline-line {
            background: linear-gradient(to right, #3B82F6, #10B981, #F59E0B);
        }
        .progress-ring {
            transition: stroke-dasharray 0.5s ease-in-out;
        }
    </style>
</head>
<body class="bg-gradient-to-br from-blue-50 to-indigo-100 min-h-screen">
    <!-- Header -->
    <header class="bg-white shadow-lg border-b-4 border-blue-600">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center py-6">
                <div class="flex items-center space-x-4">
                    <div class="w-12 h-12 bg-gradient-to-r from-blue-600 to-indigo-700 rounded-lg flex items-center justify-center">
                        <span class="text-white font-bold text-xl">MC</span>
                    </div>
                    <div>
                        <h1 class="text-3xl font-bold text-gray-900">The Moment Connect</h1>
                        <p class="text-lg text-gray-600">Development Roadmap & Technology Stack</p>
                    </div>
                </div>
                <div class="text-right">
                    <div class="text-2xl font-bold text-blue-600">12 Weeks</div>
                    <div class="text-sm text-gray-600">6 Sprints • 3 Dashboards</div>
                </div>
            </div>
        </div>
    </header>

    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8">
        <!-- Technology Stack Overview -->
        <div class="bg-white rounded-xl shadow-lg p-8 mb-8">
            <h2 class="text-2xl font-bold text-gray-900 mb-6">🛠️ Recommended Technology Stack</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Frontend -->
                <div class="bg-blue-50 rounded-lg p-6">
                    <h3 class="text-lg font-semibold text-blue-900 mb-4">Frontend</h3>
                    <div class="space-y-3">
                        <div class="tech-badge bg-blue-600 text-white px-3 py-2 rounded-lg text-sm font-medium">React.js 18+ with TypeScript</div>
                        <div class="tech-badge bg-blue-500 text-white px-3 py-2 rounded-lg text-sm font-medium">Tailwind CSS</div>
                        <div class="tech-badge bg-blue-400 text-white px-3 py-2 rounded-lg text-sm font-medium">React Query (TanStack)</div>
                        <div class="tech-badge bg-blue-300 text-white px-3 py-2 rounded-lg text-sm font-medium">React Router v6</div>
                        <div class="tech-badge bg-blue-200 text-gray-800 px-3 py-2 rounded-lg text-sm font-medium">Chart.js / Recharts</div>
                    </div>
                </div>

                <!-- Backend -->
                <div class="bg-green-50 rounded-lg p-6">
                    <h3 class="text-lg font-semibold text-green-900 mb-4">Backend</h3>
                    <div class="space-y-3">
                        <div class="tech-badge bg-green-600 text-white px-3 py-2 rounded-lg text-sm font-medium">Node.js with Express</div>
                        <div class="tech-badge bg-green-500 text-white px-3 py-2 rounded-lg text-sm font-medium">TypeScript</div>
                        <div class="tech-badge bg-green-400 text-white px-3 py-2 rounded-lg text-sm font-medium">PostgreSQL</div>
                        <div class="tech-badge bg-green-300 text-white px-3 py-2 rounded-lg text-sm font-medium">Prisma ORM</div>
                        <div class="tech-badge bg-green-200 text-gray-800 px-3 py-2 rounded-lg text-sm font-medium">Redis (Caching)</div>
                    </div>
                </div>

                <!-- Infrastructure -->
                <div class="bg-purple-50 rounded-lg p-6">
                    <h3 class="text-lg font-semibold text-purple-900 mb-4">Infrastructure</h3>
                    <div class="space-y-3">
                        <div class="tech-badge bg-purple-600 text-white px-3 py-2 rounded-lg text-sm font-medium">AWS (EC2, RDS, S3)</div>
                        <div class="tech-badge bg-purple-500 text-white px-3 py-2 rounded-lg text-sm font-medium">Docker + Kubernetes</div>
                        <div class="tech-badge bg-purple-400 text-white px-3 py-2 rounded-lg text-sm font-medium">GitHub Actions CI/CD</div>
                        <div class="tech-badge bg-purple-300 text-white px-3 py-2 rounded-lg text-sm font-medium">Auth0 (Authentication)</div>
                        <div class="tech-badge bg-purple-200 text-gray-800 px-3 py-2 rounded-lg text-sm font-medium">Socket.io (Real-time)</div>
                    </div>
                </div>
            </div>

            <!-- Architecture Highlights -->
            <div class="mt-8 grid grid-cols-1 md:grid-cols-3 gap-6">
                <div class="bg-gradient-to-r from-blue-500 to-blue-600 text-white p-6 rounded-lg">
                    <h4 class="font-semibold mb-2">🏗️ Microservices Architecture</h4>
                    <p class="text-sm opacity-90">Separate services for referrals, matching, notifications, and analytics</p>
                </div>
                <div class="bg-gradient-to-r from-green-500 to-green-600 text-white p-6 rounded-lg">
                    <h4 class="font-semibold mb-2">🔄 Real-time Updates</h4>
                    <p class="text-sm opacity-90">Live dashboard synchronization across all user roles</p>
                </div>
                <div class="bg-gradient-to-r from-purple-500 to-purple-600 text-white p-6 rounded-lg">
                    <h4 class="font-semibold mb-2">🔒 HIPAA Compliance</h4>
                    <p class="text-sm opacity-90">End-to-end encryption and audit logging</p>
                </div>
            </div>
        </div>

        <!-- Sprint Timeline -->
        <div class="bg-white rounded-xl shadow-lg p-8 mb-8">
            <div class="flex justify-between items-center mb-6">
                <h2 class="text-2xl font-bold text-gray-900">📅 Sprint Timeline (12 Weeks)</h2>
                <div class="flex items-center space-x-4">
                    <div class="text-sm text-gray-600">Progress:</div>
                    <div class="w-32 h-2 bg-gray-200 rounded-full">
                        <div class="timeline-line h-2 rounded-full" style="width: 0%" id="overall-progress"></div>
                    </div>
                    <button onclick="simulateProgress()" class="bg-blue-600 hover:bg-blue-700 text-white px-4 py-2 rounded-lg text-sm">▶ Simulate Progress</button>
                </div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Sprint 1 -->
                <div class="sprint-card bg-gradient-to-br from-blue-50 to-blue-100 rounded-lg p-6 border-l-4 border-blue-500">
                    <div class="flex justify-between items-start mb-4">
                        <div>
                            <h3 class="text-lg font-bold text-blue-900">Sprint 1</h3>
                            <p class="text-sm text-blue-700">Weeks 1-2</p>
                        </div>
                        <div class="w-12 h-12 relative">
                            <svg class="w-12 h-12 transform -rotate-90">
                                <circle cx="24" cy="24" r="20" stroke="#E5E7EB" stroke-width="4" fill="none"/>
                                <circle cx="24" cy="24" r="20" stroke="#3B82F6" stroke-width="4" fill="none" 
                                        stroke-dasharray="125.6" stroke-dashoffset="125.6" class="progress-ring" id="sprint1-progress"/>
                            </svg>
                            <div class="absolute inset-0 flex items-center justify-center text-xs font-bold text-blue-600" id="sprint1-percent">0%</div>
                        </div>
                    </div>
                    <h4 class="font-semibold text-gray-900 mb-2">🏗️ Foundation & Setup</h4>
                    <ul class="text-sm text-gray-700 space-y-1 mb-4">
                        <li>• Project setup & CI/CD pipeline</li>
                        <li>• Database schema design</li>
                        <li>• Authentication system</li>
                        <li>• Basic UI components</li>
                        <li>• Admin dashboard skeleton</li>
                    </ul>
                    <div class="bg-blue-200 text-blue-800 px-3 py-1 rounded-full text-xs font-medium">Foundation</div>
                </div>

                <!-- Sprint 2 -->
                <div class="sprint-card bg-gradient-to-br from-green-50 to-green-100 rounded-lg p-6 border-l-4 border-green-500">
                    <div class="flex justify-between items-start mb-4">
                        <div>
                            <h3 class="text-lg font-bold text-green-900">Sprint 2</h3>
                            <p class="text-sm text-green-700">Weeks 3-4</p>
                        </div>
                        <div class="w-12 h-12 relative">
                            <svg class="w-12 h-12 transform -rotate-90">
                                <circle cx="24" cy="24" r="20" stroke="#E5E7EB" stroke-width="4" fill="none"/>
                                <circle cx="24" cy="24" r="20" stroke="#10B981" stroke-width="4" fill="none" 
                                        stroke-dasharray="125.6" stroke-dashoffset="125.6" class="progress-ring" id="sprint2-progress"/>
                            </svg>
                            <div class="absolute inset-0 flex items-center justify-center text-xs font-bold text-green-600" id="sprint2-percent">0%</div>
                        </div>
                    </div>
                    <h4 class="font-semibold text-gray-900 mb-2">📝 Core Referral System</h4>
                    <ul class="text-sm text-gray-700 space-y-1 mb-4">
                        <li>• Referral submission forms</li>
                        <li>• Agency dashboard core features</li>
                        <li>• Basic referral tracking</li>
                        <li>• User role management</li>
                        <li>• Email notifications</li>
                    </ul>
                    <div class="bg-green-200 text-green-800 px-3 py-1 rounded-full text-xs font-medium">Core Features</div>
                </div>

                <!-- Sprint 3 -->
                <div class="sprint-card bg-gradient-to-br from-purple-50 to-purple-100 rounded-lg p-6 border-l-4 border-purple-500">
                    <div class="flex justify-between items-start mb-4">
                        <div>
                            <h3 class="text-lg font-bold text-purple-900">Sprint 3</h3>
                            <p class="text-sm text-purple-700">Weeks 5-6</p>
                        </div>
                        <div class="w-12 h-12 relative">
                            <svg class="w-12 h-12 transform -rotate-90">
                                <circle cx="24" cy="24" r="20" stroke="#E5E7EB" stroke-width="4" fill="none"/>
                                <circle cx="24" cy="24" r="20" stroke="#8B5CF6" stroke-width="4" fill="none" 
                                        stroke-dasharray="125.6" stroke-dashoffset="125.6" class="progress-ring" id="sprint3-progress"/>
                            </svg>
                            <div class="absolute inset-0 flex items-center justify-center text-xs font-bold text-purple-600" id="sprint3-percent">0%</div>
                        </div>
                    </div>
                    <h4 class="font-semibold text-gray-900 mb-2">🏥 Facility Management</h4>
                    <ul class="text-sm text-gray-700 space-y-1 mb-4">
                        <li>• Facility dashboard development</li>
                        <li>• Bed availability tracking</li>
                        <li>• Referral review system</li>
                        <li>• Capacity management</li>
                        <li>• Basic matching algorithm</li>
                    </ul>
                    <div class="bg-purple-200 text-purple-800 px-3 py-1 rounded-full text-xs font-medium">Facility Features</div>
                </div>

                <!-- Sprint 4 -->
                <div class="sprint-card bg-gradient-to-br from-orange-50 to-orange-100 rounded-lg p-6 border-l-4 border-orange-500">
                    <div class="flex justify-between items-start mb-4">
                        <div>
                            <h3 class="text-lg font-bold text-orange-900">Sprint 4</h3>
                            <p class="text-sm text-orange-700">Weeks 7-8</p>
                        </div>
                        <div class="w-12 h-12 relative">
                            <svg class="w-12 h-12 transform -rotate-90">
                                <circle cx="24" cy="24" r="20" stroke="#E5E7EB" stroke-width="4" fill="none"/>
                                <circle cx="24" cy="24" r="20" stroke="#F59E0B" stroke-width="4" fill="none" 
                                        stroke-dasharray="125.6" stroke-dashoffset="125.6" class="progress-ring" id="sprint4-progress"/>
                            </svg>
                            <div class="absolute inset-0 flex items-center justify-center text-xs font-bold text-orange-600" id="sprint4-percent">0%</div>
                        </div>
                    </div>
                    <h4 class="font-semibold text-gray-900 mb-2">🤖 AI Matching & Real-time</h4>
                    <ul class="text-sm text-gray-700 space-y-1 mb-4">
                        <li>• Advanced matching algorithm</li>
                        <li>• Real-time dashboard updates</li>
                        <li>• WebSocket implementation</li>
                        <li>• Automated notifications</li>
                        <li>• Performance optimization</li>
                    </ul>
                    <div class="bg-orange-200 text-orange-800 px-3 py-1 rounded-full text-xs font-medium">AI & Real-time</div>
                </div>

                <!-- Sprint 5 -->
                <div class="sprint-card bg-gradient-to-br from-red-50 to-red-100 rounded-lg p-6 border-l-4 border-red-500">
                    <div class="flex justify-between items-start mb-4">
                        <div>
                            <h3 class="text-lg font-bold text-red-900">Sprint 5</h3>
                            <p class="text-sm text-red-700">Weeks 9-10</p>
                        </div>
                        <div class="w-12 h-12 relative">
                            <svg class="w-12 h-12 transform -rotate-90">
                                <circle cx="24" cy="24" r="20" stroke="#E5E7EB" stroke-width="4" fill="none"/>
                                <circle cx="24" cy="24" r="20" stroke="#EF4444" stroke-width="4" fill="none" 
                                        stroke-dasharray="125.6" stroke-dashoffset="125.6" class="progress-ring" id="sprint5-progress"/>
                            </svg>
                            <div class="absolute inset-0 flex items-center justify-center text-xs font-bold text-red-600" id="sprint5-percent">0%</div>
                        </div>
                    </div>
                    <h4 class="font-semibold text-gray-900 mb-2">📊 Analytics & Reporting</h4>
                    <ul class="text-sm text-gray-700 space-y-1 mb-4">
                        <li>• Advanced analytics dashboard</li>
                        <li>• Custom report generation</li>
                        <li>• Performance metrics</li>
                        <li>• Data visualization</li>
                        <li>• Compliance reporting</li>
                    </ul>
                    <div class="bg-red-200 text-red-800 px-3 py-1 rounded-full text-xs font-medium">Analytics</div>
                </div>

                <!-- Sprint 6 -->
                <div class="sprint-card bg-gradient-to-br from-indigo-50 to-indigo-100 rounded-lg p-6 border-l-4 border-indigo-500">
                    <div class="flex justify-between items-start mb-4">
                        <div>
                            <h3 class="text-lg font-bold text-indigo-900">Sprint 6</h3>
                            <p class="text-sm text-indigo-700">Weeks 11-12</p>
                        </div>
                        <div class="w-12 h-12 relative">
                            <svg class="w-12 h-12 transform -rotate-90">
                                <circle cx="24" cy="24" r="20" stroke="#E5E7EB" stroke-width="4" fill="none"/>
                                <circle cx="24" cy="24" r="20" stroke="#6366F1" stroke-width="4" fill="none" 
                                        stroke-dasharray="125.6" stroke-dashoffset="125.6" class="progress-ring" id="sprint6-progress"/>
                            </svg>
                            <div class="absolute inset-0 flex items-center justify-center text-xs font-bold text-indigo-600" id="sprint6-percent">0%</div>
                        </div>
                    </div>
                    <h4 class="font-semibold text-gray-900 mb-2">🚀 Testing & Deployment</h4>
                    <ul class="text-sm text-gray-700 space-y-1 mb-4">
                        <li>• Comprehensive testing suite</li>
                        <li>• Security audit & HIPAA compliance</li>
                        <li>• Production deployment</li>
                        <li>• User training & documentation</li>
                        <li>• Go-live support</li>
                    </ul>
                    <div class="bg-indigo-200 text-indigo-800 px-3 py-1 rounded-full text-xs font-medium">Production</div>
                </div>
            </div>
        </div>

        <!-- Resource Planning -->
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 mb-8">
            <!-- Team Structure -->
            <div class="bg-white rounded-xl shadow-lg p-8">
                <h2 class="text-2xl font-bold text-gray-900 mb-6">👥 Team Structure</h2>
                <div class="space-y-4">
                    <div class="flex items-center justify-between p-4 bg-blue-50 rounded-lg">
                        <div class="flex items-center space-x-3">
                            <div class="w-10 h-10 bg-blue-600 rounded-full flex items-center justify-center">
                                <span class="text-white font-bold text-sm">PM</span>
                            </div>
                            <div>
                                <div class="font-semibold text-gray-900">Project Manager</div>
                                <div class="text-sm text-gray-600">Agile coordination & stakeholder management</div>
                            </div>
                        </div>
                        <div class="text-blue-600 font-bold">1</div>
                    </div>
                    
                    <div class="flex items-center justify-between p-4 bg-green-50 rounded-lg">
                        <div class="flex items-center space-x-3">
                            <div class="w-10 h-10 bg-green-600 rounded-full flex items-center justify-center">
                                <span class="text-white font-bold text-sm">FS</span>
                            </div>
                            <div>
                                <div class="font-semibold text-gray-900">Full-Stack Developers</div>
                                <div class="text-sm text-gray-600">React, Node.js, database development</div>
                            </div>
                        </div>
                        <div class="text-green-600 font-bold">3</div>
                    </div>
                    
                    <div class="flex items-center justify-between p-4 bg-purple-50 rounded-lg">
                        <div class="flex items-center space-x-3">
                            <div class="w-10 h-10 bg-purple-600 rounded-full flex items-center justify-center">
                                <span class="text-white font-bold text-sm">FE</span>
                            </div>
                            <div>
                                <div class="font-semibold text-gray-900">Frontend Specialist</div>
                                <div class="text-sm text-gray-600">UI/UX implementation & optimization</div>
                            </div>
                        </div>
                        <div class="text-purple-600 font-bold">1</div>
                    </div>
                    
                    <div class="flex items-center justify-between p-4 bg-orange-50 rounded-lg">
                        <div class="flex items-center space-x-3">
                            <div class="w-10 h-10 bg-orange-600 rounded-full flex items-center justify-center">
                                <span class="text-white font-bold text-sm">DO</span>
                            </div>
                            <div>
                                <div class="font-semibold text-gray-900">DevOps Engineer</div>
                                <div class="text-sm text-gray-600">Infrastructure, deployment, monitoring</div>
                            </div>
                        </div>
                        <div class="text-orange-600 font-bold">1</div>
                    </div>
                    
                    <div class="flex items-center justify-between p-4 bg-red-50 rounded-lg">
                        <div class="flex items-center space-x-3">
                            <div class="w-10 h-10 bg-red-600 rounded-full flex items-center justify-center">
                                <span class="text-white font-bold text-sm">QA</span>
                            </div>
                            <div>
                                <div class="font-semibold text-gray-900">QA Engineer</div>
                                <div class="text-sm text-gray-600">Testing, automation, quality assurance</div>
                            </div>
                        </div>
                        <div class="text-red-600 font-bold">1</div>
                    </div>
                </div>
                
                <div class="mt-6 pt-6 border-t border-gray-200">
                    <div class="flex justify-between items-center">
                        <span class="font-semibold text-gray-900">Total Team Size</span>
                        <span class="text-2xl font-bold text-blue-600">7 People</span>
                    </div>
                </div>
            </div>

            <!-- Budget & Timeline -->
            <div class="bg-white rounded-xl shadow-lg p-8">
                <h2 class="text-2xl font-bold text-gray-900 mb-6">💰 Budget & Timeline</h2>
                
                <div class="space-y-6">
                    <div class="bg-gradient-to-r from-blue-500 to-blue-600 text-white p-6 rounded-lg">
                        <h3 class="font-semibold mb-2">Development Cost</h3>
                        <div class="text-3xl font-bold">$240K - $320K</div>
                        <div class="text-sm opacity-90">Based on team size and timeline</div>
                    </div>
                    
                    <div class="bg-gradient-to-r from-green-500 to-green-600 text-white p-6 rounded-lg">
                        <h3 class="font-semibold mb-2">Timeline</h3>
                        <div class="text-3xl font-bold">12 Weeks</div>
                        <div class="text-sm opacity-90">6 sprints × 2 weeks each</div>
                    </div>
                    
                    <div class="bg-gradient-to-r from-purple-500 to-purple-600 text-white p-6 rounded-lg">
                        <h3 class="font-semibold mb-2">Infrastructure (Annual)</h3>
                        <div class="text-3xl font-bold">$24K - $36K</div>
                        <div class="text-sm opacity-90">AWS hosting, monitoring, security</div>
                    </div>
                </div>
                
                <div class="mt-6 p-4 bg-gray-50 rounded-lg">
                    <h4 class="font-semibold text-gray-900 mb-2">Cost Breakdown</h4>
                    <div class="space-y-2 text-sm">
                        <div class="flex justify-between">
                            <span>Development Team (12 weeks)</span>
                            <span>$200K - $280K</span>
                        </div>
                        <div class="flex justify-between">
                            <span>Project Management</span>
                            <span>$20K - $25K</span>
                        </div>
                        <div class="flex justify-between">
                            <span>Tools & Licenses</span>
                            <span>$10K - $15K</span>
                        </div>
                        <div class="flex justify-between">
                            <span>Testing & QA</span>
                            <span>$10K - $15K</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Key Features by Sprint -->
        <div class="bg-white rounded-xl shadow-lg p-8">
            <h2 class="text-2xl font-bold text-gray-900 mb-6">🎯 Key Features by Sprint</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Admin Dashboard Features -->
                <div class="space-y-4">
                    <h3 class="text-lg font-bold text-blue-600 flex items-center">
                        <span class="w-8 h-8 bg-blue-600 text-white rounded-full flex items-center justify-center text-sm mr-2">A</span>
                        Admin Dashboard
                    </h3>
                    <div class="space-y-3">
                        <div class="p-3 bg-blue-50 rounded-lg">
                            <div class="font-medium text-gray-900">Sprint 1-2</div>
                            <div class="text-sm text-gray-600">User management, system monitoring, basic analytics</div>
                        </div>
                        <div class="p-3 bg-blue-50 rounded-lg">
                            <div class="font-medium text-gray-900">Sprint 3-4</div>
                            <div class="text-sm text-gray-600">Referral oversight, matching approval, escalation handling</div>
                        </div>
                        <div class="p-3 bg-blue-50 rounded-lg">
                            <div class="font-medium text-gray-900">Sprint 5-6</div>
                            <div class="text-sm text-gray-600">Advanced reporting, compliance tools, performance metrics</div>
                        </div>
                    </div>
                </div>

                <!-- Agency Dashboard Features -->
                <div class="space-y-4">
                    <h3 class="text-lg font-bold text-green-600 flex items-center">
                        <span class="w-8 h-8 bg-green-600 text-white rounded-full flex items-center justify-center text-sm mr-2">G</span>
                        Agency Dashboard
                    </h3>
                    <div class="space-y-3">
                        <div class="p-3 bg-green-50 rounded-lg">
                            <div class="font-medium text-gray-900">Sprint 1-2</div>
                            <div class="text-sm text-gray-600">Referral submission, client tracking, basic notifications</div>
                        </div>
                        <div class="p-3 bg-green-50 rounded-lg">
                            <div class="font-medium text-gray-900">Sprint 3-4</div>
                            <div class="text-sm text-gray-600">Real-time status updates, facility communication, case management</div>
                        </div>
                        <div class="p-3 bg-green-50 rounded-lg">
                            <div class="font-medium text-gray-900">Sprint 5-6</div>
                            <div class="text-sm text-gray-600">Performance analytics, outcome tracking, custom reports</div>
                        </div>
                    </div>
                </div>

                <!-- Facility Dashboard Features -->
                <div class="space-y-4">
                    <h3 class="text-lg font-bold text-orange-600 flex items-center">
                        <span class="w-8 h-8 bg-orange-600 text-white rounded-full flex items-center justify-center text-sm mr-2">F</span>
                        Facility Dashboard
                    </h3>
                    <div class="space-y-3">
                        <div class="p-3 bg-orange-50 rounded-lg">
                            <div class="font-medium text-gray-900">Sprint 1-2</div>
                            <div class="text-sm text-gray-600">Bed management, basic referral review, capacity tracking</div>
                        </div>
                        <div class="p-3 bg-orange-50 rounded-lg">
                            <div class="font-medium text-gray-900">Sprint 3-4</div>
                            <div class="text-sm text-gray-600">Advanced matching, admission workflow, real-time updates</div>
                        </div>
                        <div class="p-3 bg-orange-50 rounded-lg">
                            <div class="font-medium text-gray-900">Sprint 5-6</div>
                            <div class="text-sm text-gray-600">Occupancy analytics, outcome reporting, integration tools</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        let progressInterval;
        let currentProgress = 0;

        function simulateProgress() {
            if (progressInterval) {
                clearInterval(progressInterval);
                resetProgress();
                return;
            }

            const button = document.querySelector('button[onclick="simulateProgress()"]');
            button.textContent = '⏸ Stop Simulation';
            button.classList.remove('bg-blue-600', 'hover:bg-blue-700');
            button.classList.add('bg-red-600', 'hover:bg-red-700');

            progressInterval = setInterval(() => {
                currentProgress += 2;
                
                // Update overall progress
                document.getElementById('overall-progress').style.width = `${Math.min(currentProgress, 100)}%`;
                
                // Update individual sprint progress
                const sprintProgress = Math.max(0, Math.min(100, (currentProgress - (Math.floor(currentProgress / 17) * 17)) * 6));
                const currentSprint = Math.floor(currentProgress / 17) + 1;
                
                for (let i = 1; i <= 6; i++) {
                    const ring = document.getElementById(`sprint${i}-progress`);
                    const percent = document.getElementById(`sprint${i}-percent`);
                    
                    if (i < currentSprint) {
                        // Completed sprints
                        ring.style.strokeDashoffset = '0';
                        percent.textContent = '100%';
                    } else if (i === currentSprint) {
                        // Current sprint
                        const offset = 125.6 - (125.6 * sprintProgress / 100);
                        ring.style.strokeDashoffset = offset;
                        percent.textContent = `${Math.round(sprintProgress)}%`;
                    } else {
                        // Future sprints
                        ring.style.strokeDashoffset = '125.6';
                        percent.textContent = '0%';
                    }
                }
                
                if (currentProgress >= 100) {
                    clearInterval(progressInterval);
                    progressInterval = null;
                    button.textContent = '🎉 Completed!';
                    button.classList.remove('bg-red-600', 'hover:bg-red-700');
                    button.classList.add('bg-green-600', 'hover:bg-green-700');
                    
                    setTimeout(() => {
                        button.textContent = '▶ Simulate Progress';
                        button.classList.remove('bg-green-600', 'hover:bg-green-700');
                        button.classList.add('bg-blue-600', 'hover:bg-blue-700');
                    }, 3000);
                }
            }, 100);
        }

        function resetProgress() {
            currentProgress = 0;
            document.getElementById('overall-progress').style.width = '0%';
            
            for (let i = 1; i <= 6; i++) {
                document.getElementById(`sprint${i}-progress`).style.strokeDashoffset = '125.6';
                document.getElementById(`sprint${i}-percent`).textContent = '0%';
            }
            
            const button = document.querySelector('button[onclick="simulateProgress()"]');
            button.textContent = '▶ Simulate Progress';
            button.classList.remove('bg-red-600', 'hover:bg-red-700', 'bg-green-600', 'hover:bg-green-700');
            button.classList.add('bg-blue-600', 'hover:bg-blue-700');
            
            progressInterval = null;
        }

        // Add hover effects to sprint cards
        document.querySelectorAll('.sprint-card').forEach(card => {
            card.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-4px) scale(1.02)';
            });
            
            card.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0) scale(1)';
            });
        });
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'989a7744c0a52cba',t:'MTc1OTY0MTU4NS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
