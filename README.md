import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Tabs, TabsContent, TabsList, TabsTrigger } from "@/components/ui/tabs";
import { ScrollArea } from "@/components/ui/scroll-area";

export default function Portfolio() {
  return (
    <div className="p-6 max-w-5xl mx-auto">
      <h1 className="text-4xl font-bold mb-2">Jazzer M. Manuta</h1>
      <p className="text-lg text-gray-600 mb-6">Tech-Savvy IT Graduate | Results-Driven & Adaptable</p>
      <div className="text-sm text-gray-500 mb-6">
        <p>📍 Sabayle St., Iligan City</p>
        <p>📞 +63 912 9155 891</p>
      </div>

      <Tabs defaultValue="summary" className="w-full">
        <TabsList className="grid grid-cols-4 mb-4">
          <TabsTrigger value="summary">Summary</TabsTrigger>
          <TabsTrigger value="experience">Experience</TabsTrigger>
          <TabsTrigger value="education">Education</TabsTrigger>
          <TabsTrigger value="training">Training</TabsTrigger>
        </TabsList>

        <ScrollArea className="h-[500px]">
          <TabsContent value="summary">
            <Card>
              <CardContent className="p-4 space-y-4">
                <h2 className="text-xl font-semibold">Value Statement</h2>
                <p>I am an adaptable and results-oriented IT graduate with a strong foundation in programming, digital tools, and administrative functions...</p>

                <h2 className="text-xl font-semibold">Summary of Qualifications</h2>
                <ul className="list-disc list-inside space-y-1">
                  <li>Equipped with high-performance devices and backup systems</li>
                  <li>Skilled in Python, Java, C++, HTML</li>
                  <li>Experienced in Adobe, WordPress, Microsoft Office, and more</li>
                  <li>Business management and e-commerce experience</li>
                  <li>Strong communication in English, Cebuano, Tagalog</li>
                  <li>Typing speed of 60+ WPM</li>
                </ul>

                <h2 className="text-xl font-semibold">Soft Skills</h2>
                <p>Adaptability, Attention to detail, Multi-tasking, Diligence, Flexibility, Critical Thinking, Emotional Intelligence, Time Management</p>
              </CardContent>
            </Card>
          </TabsContent>

          <TabsContent value="experience">
            <Card>
              <CardContent className="p-4 space-y-4">
                <h2 className="text-xl font-semibold">Work Experience</h2>
                <ul className="space-y-3">
                  <li>
                    <strong>Network Marketing Business Associate</strong> – Maximum88 (2018)<br/>
                    Expanded networks through online marketing and mentoring.
                  </li>
                  <li>
                    <strong>Online Business Owner</strong> – Exclusive FB Store (2016–2017)<br/>
                    Managed inventory, customer engagement, and marketing.
                  </li>
                  <li>
                    <strong>Bicycle Shop Manager</strong> – AJ Bicycle Trading (2017–2022)<br/>
                    Oversaw operations, audits, inventory, and customer service.
                  </li>
                </ul>
              </CardContent>
            </Card>
          </TabsContent>

          <TabsContent value="education">
            <Card>
              <CardContent className="p-4 space-y-4">
                <h2 className="text-xl font-semibold">Education</h2>
                <ul className="space-y-2">
                  <li><strong>BS in Information Technology</strong>, ICI Iligan (2012–2015)</li>
                  <li><strong>High School</strong>, St. Peter’s College (2006–2009)</li>
                  <li><strong>Elementary</strong>, St. Paul’s Institute of Technology (2000–2005)</li>
                </ul>

                <h2 className="text-xl font-semibold">IT Coursework</h2>
                <ul className="list-disc list-inside">
                  <li>Programming, Data Structures & Algorithms</li>
                  <li>Database Management, Networking</li>
                  <li>Digital Marketing, E-commerce, Web Development</li>
                </ul>
              </CardContent>
            </Card>
          </TabsContent>

          <TabsContent value="training">
            <Card>
              <CardContent className="p-4 space-y-4">
                <h2 className="text-xl font-semibold">Relevant Training & Seminars</h2>
                <ul className="list-disc list-inside space-y-2">
                  <li>Virtual Assistant Course – Home-based Connect (2020)</li>
                  <li>Email Marketing & Copywriting – Pagulayan & Ngo (2023)</li>
                  <li>Advanced Digital System – Project Multiply (2023)</li>
                  <li>Culture in the Workplace – St. Michael’s College (2021)</li>
                </ul>

                <h2 className="text-xl font-semibold">Personal Info</h2>
                <p>Age: 29 | Gender: Male | Birthday: Nov 18, 1993 | Nationality: Filipino | Married | Religion: Roman Catholic</p>
              </CardContent>
            </Card>
          </TabsContent>
        </ScrollArea>
      </Tabs>
    </div>
  );
}


