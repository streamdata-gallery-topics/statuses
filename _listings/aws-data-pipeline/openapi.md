swagger: "2.0"
x-collection-name: AWS Data Pipeline
x-complete: 1
info:
  title: AWS Data Pipeline API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=SetStatus:
    get:
      summary: Set Status
      description: Requests that the status of the specified physical or logical pipeline
        objects be updated in the specified pipeline.
      operationId: setStatus
      x-api-path-slug: actionsetstatus-get
      parameters:
      - in: query
        name: objectIds
        description: The IDs of the objects
        type: string
      - in: query
        name: pipelineId
        description: The ID of the pipeline that contains the objects
        type: string
      - in: query
        name: status
        description: The status to be set on all the objects specified in objectIds
        type: string
      responses:
        200:
          description: OK
      tags:
      - Status
  /?Action=SetTaskStatus:
    get:
      summary: Set Task Status
      description: Task runners call SetTaskStatus to notify AWS Data Pipeline that
        a task is completed and provide information about the final status.
      operationId: setTaskStatus
      x-api-path-slug: actionsettaskstatus-get
      parameters:
      - in: query
        name: errorId
        description: If an error occurred during the task, this value specifies the
          error code
        type: string
      - in: query
        name: errorMessage
        description: If an error occurred during the task, this value specifies a
          text description of the error
        type: string
      - in: query
        name: errorStackTrace
        description: If an error occurred during the task, this value specifies the
          stack trace associated with the error
        type: string
      - in: query
        name: taskId
        description: The ID of the task assigned to the task runner
        type: string
      - in: query
        name: taskStatus
        description: If FINISHED, the task successfully completed
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tasks