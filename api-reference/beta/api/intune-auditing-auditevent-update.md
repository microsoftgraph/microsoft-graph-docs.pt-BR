---
title: Atualizar auditEvent
description: Atualizar as propriedades do objeto auditEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1dc5508ac19e81017eb46a5e8e812d304802f736
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085138"
---
# <a name="update-auditevent"></a><span data-ttu-id="406c4-103">Atualizar auditEvent</span><span class="sxs-lookup"><span data-stu-id="406c4-103">Update auditEvent</span></span>

> <span data-ttu-id="406c4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="406c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="406c4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="406c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="406c4-106">Atualizar as propriedades do objeto [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="406c4-106">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="406c4-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="406c4-107">Prerequisites</span></span>
<span data-ttu-id="406c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="406c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="406c4-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="406c4-110">Permission type</span></span>|<span data-ttu-id="406c4-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="406c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="406c4-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="406c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="406c4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="406c4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="406c4-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="406c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="406c4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="406c4-115">Not supported.</span></span>|
|<span data-ttu-id="406c4-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="406c4-116">Application</span></span>|<span data-ttu-id="406c4-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="406c4-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="406c4-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="406c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="406c4-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="406c4-119">Request headers</span></span>
|<span data-ttu-id="406c4-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="406c4-120">Header</span></span>|<span data-ttu-id="406c4-121">Valor</span><span class="sxs-lookup"><span data-stu-id="406c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="406c4-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="406c4-122">Authorization</span></span>|<span data-ttu-id="406c4-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="406c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="406c4-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="406c4-124">Accept</span></span>|<span data-ttu-id="406c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="406c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="406c4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="406c4-126">Request body</span></span>
<span data-ttu-id="406c4-127">No corpo da solicitação, forneça uma representação JSON do objeto [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="406c4-127">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="406c4-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="406c4-128">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="406c4-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="406c4-129">Property</span></span>|<span data-ttu-id="406c4-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="406c4-130">Type</span></span>|<span data-ttu-id="406c4-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="406c4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="406c4-132">id</span><span class="sxs-lookup"><span data-stu-id="406c4-132">id</span></span>|<span data-ttu-id="406c4-133">String</span><span class="sxs-lookup"><span data-stu-id="406c4-133">String</span></span>|<span data-ttu-id="406c4-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="406c4-134">Key of the entity.</span></span>|
|<span data-ttu-id="406c4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="406c4-135">displayName</span></span>|<span data-ttu-id="406c4-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="406c4-136">String</span></span>|<span data-ttu-id="406c4-137">Nome de exibição do evento.</span><span class="sxs-lookup"><span data-stu-id="406c4-137">Event display name.</span></span>|
|<span data-ttu-id="406c4-138">componentName</span><span class="sxs-lookup"><span data-stu-id="406c4-138">componentName</span></span>|<span data-ttu-id="406c4-139">String</span><span class="sxs-lookup"><span data-stu-id="406c4-139">String</span></span>|<span data-ttu-id="406c4-140">Nome do componente.</span><span class="sxs-lookup"><span data-stu-id="406c4-140">Component name.</span></span>|
|<span data-ttu-id="406c4-141">actor</span><span class="sxs-lookup"><span data-stu-id="406c4-141">actor</span></span>|[<span data-ttu-id="406c4-142">auditActor</span><span class="sxs-lookup"><span data-stu-id="406c4-142">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="406c4-143">Usuários e aplicativos do AAD associados com o evento de auditoria.</span><span class="sxs-lookup"><span data-stu-id="406c4-143">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="406c4-144">atividade</span><span class="sxs-lookup"><span data-stu-id="406c4-144">activity</span></span>|<span data-ttu-id="406c4-145">String</span><span class="sxs-lookup"><span data-stu-id="406c4-145">String</span></span>|<span data-ttu-id="406c4-146">Nome amigável da atividade.</span><span class="sxs-lookup"><span data-stu-id="406c4-146">Friendly name of the activity.</span></span>|
|<span data-ttu-id="406c4-147">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="406c4-147">activityDateTime</span></span>|<span data-ttu-id="406c4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="406c4-148">DateTimeOffset</span></span>|<span data-ttu-id="406c4-149">A hora e data em UTC em que a atividade foi executada.</span><span class="sxs-lookup"><span data-stu-id="406c4-149">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="406c4-150">activityType</span><span class="sxs-lookup"><span data-stu-id="406c4-150">activityType</span></span>|<span data-ttu-id="406c4-151">String</span><span class="sxs-lookup"><span data-stu-id="406c4-151">String</span></span>|<span data-ttu-id="406c4-152">O tipo de atividade que foi executada.</span><span class="sxs-lookup"><span data-stu-id="406c4-152">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="406c4-153">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="406c4-153">activityOperationType</span></span>|<span data-ttu-id="406c4-154">String</span><span class="sxs-lookup"><span data-stu-id="406c4-154">String</span></span>|<span data-ttu-id="406c4-155">O tipo de operação HTTP da atividade.</span><span class="sxs-lookup"><span data-stu-id="406c4-155">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="406c4-156">activityResult</span><span class="sxs-lookup"><span data-stu-id="406c4-156">activityResult</span></span>|<span data-ttu-id="406c4-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="406c4-157">String</span></span>|<span data-ttu-id="406c4-158">O resultado da atividade.</span><span class="sxs-lookup"><span data-stu-id="406c4-158">The result of the activity.</span></span>|
|<span data-ttu-id="406c4-159">correlationId</span><span class="sxs-lookup"><span data-stu-id="406c4-159">correlationId</span></span>|<span data-ttu-id="406c4-160">Guid</span><span class="sxs-lookup"><span data-stu-id="406c4-160">Guid</span></span>|<span data-ttu-id="406c4-161">A ID da solicitação de cliente usada para correlacionar a atividade dentro do sistema.</span><span class="sxs-lookup"><span data-stu-id="406c4-161">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="406c4-162">recursos</span><span class="sxs-lookup"><span data-stu-id="406c4-162">resources</span></span>|<span data-ttu-id="406c4-163">Coleção [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="406c4-163">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="406c4-164">Recursos em modificação.</span><span class="sxs-lookup"><span data-stu-id="406c4-164">Resources being modified.</span></span>|
|<span data-ttu-id="406c4-165">category</span><span class="sxs-lookup"><span data-stu-id="406c4-165">category</span></span>|<span data-ttu-id="406c4-166">String</span><span class="sxs-lookup"><span data-stu-id="406c4-166">String</span></span>|<span data-ttu-id="406c4-167">Categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="406c4-167">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="406c4-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="406c4-168">Response</span></span>
<span data-ttu-id="406c4-169">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [auditEvent](../resources/intune-auditing-auditevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="406c4-169">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="406c4-170">Exemplo</span><span class="sxs-lookup"><span data-stu-id="406c4-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="406c4-171">Solicitação</span><span class="sxs-lookup"><span data-stu-id="406c4-171">Request</span></span>
<span data-ttu-id="406c4-172">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="406c4-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
Content-type: application/json
Content-length: 1603

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.roleScopeTagInfo",
        "displayName": "Display Name value",
        "roleScopeTagId": "Role Scope Tag Id value"
      }
    ]
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```

### <a name="response"></a><span data-ttu-id="406c4-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="406c4-173">Response</span></span>
<span data-ttu-id="406c4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="406c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1652

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value",
    "userRoleScopeTags": [
      {
        "@odata.type": "microsoft.graph.roleScopeTagInfo",
        "displayName": "Display Name value",
        "roleScopeTagId": "Role Scope Tag Id value"
      }
    ]
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```






