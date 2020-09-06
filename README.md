# Gantt-Viewer-for-solution-of-Rehabilitation-routing-and-scheduling-problem
A practical Gantt Viewer for a solution of Rehabilitation Routing and Scheduling problem

# Description of Solution Instance (see [instance_demo](https://github.com/martinWANG2014/Gantt-Viewer-for-solution-of-Rehabilitation-routing-and-scheduling-problem/blob/master/instance_demo.gantt)). 
>> Gantt 
>>> Gantt is a key word captured by viewer application, content before Gantt is omitted automatically.

>> Number of therapists

>> Number of patients

>> List of Id of therapists, separated by space.

>> List of Id of patients, separated by space.

>> List of Start time for therapists, separated by space.

>> List of End time for therapists, separatad by space.

>> List of Start time for patients, separated by space.

>> List of End time for patients, separated by space.

// for each therapist

>> Id of therapist and Nb of treatments served by this therapist, separated by space.

  // for each treatment served by corresponding therapist.
  
  >> Id of patient served by this therapist, start time of treatment and end time of treatment, separated by space.
  
// for each patient

>> Id of patient and Nb of treatments required by this patient, separated by space.

  // for each treatment required by corresponding patient.
  
  >> Id of therapist serving this patient, start time of treatment, end time of treatment, time travelling from previous therapist, time travelling to next therapist, and relax time after treatment, separated by space.
  
# Run viewer
>> python viewer.py or python viewer scale_factor
>>> The scale factor is a real number
# Snapshot for viewer solution
## The application is scrollable and draggable, can also zoom in and zoom out for visualization. 
>> When mouse closing the treatment a tips of details will show systematically, and is hidden after mouse leaving.

>> A general view for scheduling of therapists.
![view for therapists](https://github.com/martinWANG2014/Gantt-Viewer-for-solution-of-Rehabilitation-routing-and-scheduling-problem/blob/master/view_therapist.png)

>>> Focus on a patient by left clicking the treatment on scheduling of therapists, then all associated treatments required by patient of the selected treatment will be shown, others will be hidden. Right click to any treatment of these present treatments, will turn back to main view of scheduling of therapists.
![details for a patient](https://github.com/martinWANG2014/Gantt-Viewer-for-solution-of-Rehabilitation-routing-and-scheduling-problem/blob/master/details_patient.png)

>> A general view for scheduling of patients.
![view for patients](https://github.com/martinWANG2014/Gantt-Viewer-for-solution-of-Rehabilitation-routing-and-scheduling-problem/blob/master/view_patients.png)

