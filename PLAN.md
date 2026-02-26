# Project Plan

<!-- veritas-normalized 2026-02-25 prefix=F42 source=README.md -->

## Feature: Contents [ID=F42-01]

## Feature: cloned-repos ? Reference Repositories [ID=F42-02]

## Feature: spikes/ [ID=F42-03]

## Feature: API API [ID=F42-API]

### Story: GET / [ID=F42-API-001]

### Story: GET / [ID=F42-API-002]

### Story: GET / [ID=F42-API-003]

### Story: GET / [ID=F42-API-004]

### Story: GET / [ID=F42-API-005]

## Feature: CREATE_RESPO API [ID=F42-CREATE_RESPO]

### Story: POST /api/create_response [ID=F42-CREATE_RESPO-001]

## Feature: ARTICLE API [ID=F42-ARTICLE]

### Story: POST /api/article [ID=F42-ARTICLE-001]

## Feature: UPLOADIMAGE API [ID=F42-UPLOADIMAGE]

### Story: POST /api/upload-image [ID=F42-UPLOADIMAGE-001]

## Feature: USER_BROWSER API [ID=F42-USER_BROWSER]

### Story: POST /api/user_browser_language [ID=F42-USER_BROWSER-001]

## Feature: CONFIG API [ID=F42-CONFIG]

### Story: GET /config [ID=F42-CONFIG-001]

## Feature: FULL_PATHPAT API [ID=F42-FULL_PATHPAT]

### Story: GET /{full_path:path} [ID=F42-FULL_PATHPAT-001]

## Feature: HEALTH API [ID=F42-HEALTH]

### Story: GET /health [ID=F42-HEALTH-001]

## Feature: META API [ID=F42-META]

### Story: GET /meta [ID=F42-META-001]

## Feature: ENTITIES API [ID=F42-ENTITIES]

### Story: GET /v1/entities [ID=F42-ENTITIES-001]

### Story: GET /v1/entities/{entity_id}/info [ID=F42-ENTITIES-002]

### Story: POST /v1/entities/{entity_id}/reload [ID=F42-ENTITIES-003]

### Story: POST /v1/entities/{entity_id}/deploy [ID=F42-ENTITIES-004]

## Feature: DEPLOYMENTS API [ID=F42-DEPLOYMENTS]

### Story: POST /v1/deployments [ID=F42-DEPLOYMENTS-001]

### Story: GET /v1/deployments [ID=F42-DEPLOYMENTS-002]

### Story: GET /v1/deployments/{deployment_id} [ID=F42-DEPLOYMENTS-003]

### Story: DELETE /v1/deployments/{deployment_id} [ID=F42-DEPLOYMENTS-004]

## Feature: RESPONSES API [ID=F42-RESPONSES]

### Story: POST /v1/responses [ID=F42-RESPONSES-001]

### Story: POST /v1/responses/{response_id}/cancel [ID=F42-RESPONSES-002]

## Feature: CONVERSATION API [ID=F42-CONVERSATION]

### Story: POST /v1/conversations [ID=F42-CONVERSATION-001]

### Story: GET /v1/conversations [ID=F42-CONVERSATION-002]

### Story: GET /v1/conversations/{conversation_id} [ID=F42-CONVERSATION-003]

### Story: POST /v1/conversations/{conversation_id} [ID=F42-CONVERSATION-004]

### Story: DELETE /v1/conversations/{conversation_id} [ID=F42-CONVERSATION-005]

### Story: POST /v1/conversations/{conversation_id}/items [ID=F42-CONVERSATION-006]

### Story: GET /v1/conversations/{conversation_id}/items [ID=F42-CONVERSATION-007]

### Story: GET /v1/conversations/{conversation_id}/items/{item_id} [ID=F42-CONVERSATION-008]

### Story: DELETE /v1/conversations/{conversation_id}/items/{item_id} [ID=F42-CONVERSATION-009]

## Feature: CHATKIT API [ID=F42-CHATKIT]

### Story: POST /chatkit [ID=F42-CHATKIT-001]

## Feature: UPLOAD API [ID=F42-UPLOAD]

### Story: POST /upload/{attachment_id} [ID=F42-UPLOAD-001]

## Feature: PREVIEW API [ID=F42-PREVIEW]

### Story: GET /preview/{attachment_id} [ID=F42-PREVIEW-001]

## Feature: STREAM API [ID=F42-STREAM]

### Story: GET /stream [ID=F42-STREAM-001]

## Feature: MCP API [ID=F42-MCP]

### Story: POST /mcp [ID=F42-MCP-001]

### Story: GET /mcp [ID=F42-MCP-002]

### Story: DELETE /mcp [ID=F42-MCP-003]

### Story: POST /mcp [ID=F42-MCP-004]

## Feature: UI Pages [ID=F42-UI]

### Story: Route /plan/:planId [ID=F42-UI-001]

## Feature: Operations Scripts [ID=F42-OPS]

### Story: merge_principal_ids() [ID=F42-OPS-001]

### Story: log_verbose() [ID=F42-OPS-002]

### Story: restore_network_access() [ID=F42-OPS-003]

### Story: cleanup_on_exit() [ID=F42-OPS-004]

### Story: test_azd_installed() [ID=F42-OPS-005]

### Story: get_values_from_azd_env() [ID=F42-OPS-006]

### Story: extract_value() [ID=F42-OPS-007]

### Story: get_values_from_az_deployment() [ID=F42-OPS-008]

### Story: get_values_using_solution_suffix() [ID=F42-OPS-009]

### Story: configure_nssdb() [ID=F42-OPS-010]
