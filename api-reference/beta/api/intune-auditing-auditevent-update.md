---
title: Atualizar auditEvent
description: Atualizar as propriedades do objeto auditEvent.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3a4b4a0e2ef8355450f039608a7769a613296cc2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42450388"
---
# <a name="update-auditevent"></a><span data-ttu-id="f3f2e-103">Atualizar auditEvent</span><span class="sxs-lookup"><span data-stu-id="f3f2e-103">Update auditEvent</span></span>

<span data-ttu-id="f3f2e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f3f2e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3f2e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3f2e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3f2e-107">Atualizar as propriedades do objeto [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="f3f2e-107">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3f2e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f3f2e-108">Prerequisites</span></span>
<span data-ttu-id="f3f2e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f3f2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3f2e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f3f2e-111">Permission type</span></span>|<span data-ttu-id="f3f2e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f3f2e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3f2e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f3f2e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f3f2e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3f2e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f3f2e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f3f2e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3f2e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-116">Not supported.</span></span>|
|<span data-ttu-id="f3f2e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f3f2e-117">Application</span></span>|<span data-ttu-id="f3f2e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3f2e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3f2e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f3f2e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="f3f2e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f3f2e-120">Request headers</span></span>
|<span data-ttu-id="f3f2e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f3f2e-121">Header</span></span>|<span data-ttu-id="f3f2e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f3f2e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3f2e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f3f2e-123">Authorization</span></span>|<span data-ttu-id="f3f2e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3f2e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f3f2e-125">Accept</span></span>|<span data-ttu-id="f3f2e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f3f2e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3f2e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f3f2e-127">Request body</span></span>
<span data-ttu-id="f3f2e-128">No corpo da solicitação, forneça uma representação JSON do objeto [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="f3f2e-128">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="f3f2e-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="f3f2e-129">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="f3f2e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3f2e-130">Property</span></span>|<span data-ttu-id="f3f2e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3f2e-131">Type</span></span>|<span data-ttu-id="f3f2e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3f2e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3f2e-133">id</span><span class="sxs-lookup"><span data-stu-id="f3f2e-133">id</span></span>|<span data-ttu-id="f3f2e-134">String</span><span class="sxs-lookup"><span data-stu-id="f3f2e-134">String</span></span>|<span data-ttu-id="f3f2e-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-135">Key of the entity.</span></span>|
|<span data-ttu-id="f3f2e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f3f2e-136">displayName</span></span>|<span data-ttu-id="f3f2e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3f2e-137">String</span></span>|<span data-ttu-id="f3f2e-138">Nome de exibição do evento.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-138">Event display name.</span></span>|
|<span data-ttu-id="f3f2e-139">componentName</span><span class="sxs-lookup"><span data-stu-id="f3f2e-139">componentName</span></span>|<span data-ttu-id="f3f2e-140">String</span><span class="sxs-lookup"><span data-stu-id="f3f2e-140">String</span></span>|<span data-ttu-id="f3f2e-141">Nome do componente.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-141">Component name.</span></span>|
|<span data-ttu-id="f3f2e-142">actor</span><span class="sxs-lookup"><span data-stu-id="f3f2e-142">actor</span></span>|[<span data-ttu-id="f3f2e-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="f3f2e-143">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="f3f2e-144">Usuários e aplicativos do AAD associados com o evento de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="f3f2e-145">atividade</span><span class="sxs-lookup"><span data-stu-id="f3f2e-145">activity</span></span>|<span data-ttu-id="f3f2e-146">String</span><span class="sxs-lookup"><span data-stu-id="f3f2e-146">String</span></span>|<span data-ttu-id="f3f2e-147">Nome amigável da atividade.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="f3f2e-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="f3f2e-148">activityDateTime</span></span>|<span data-ttu-id="f3f2e-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3f2e-149">DateTimeOffset</span></span>|<span data-ttu-id="f3f2e-150">A hora e data em UTC em que a atividade foi executada.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="f3f2e-151">activityType</span><span class="sxs-lookup"><span data-stu-id="f3f2e-151">activityType</span></span>|<span data-ttu-id="f3f2e-152">String</span><span class="sxs-lookup"><span data-stu-id="f3f2e-152">String</span></span>|<span data-ttu-id="f3f2e-153">O tipo de atividade que foi executada.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="f3f2e-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="f3f2e-154">activityOperationType</span></span>|<span data-ttu-id="f3f2e-155">String</span><span class="sxs-lookup"><span data-stu-id="f3f2e-155">String</span></span>|<span data-ttu-id="f3f2e-156">O tipo de operação HTTP da atividade.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="f3f2e-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="f3f2e-157">activityResult</span></span>|<span data-ttu-id="f3f2e-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f3f2e-158">String</span></span>|<span data-ttu-id="f3f2e-159">O resultado da atividade.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-159">The result of the activity.</span></span>|
|<span data-ttu-id="f3f2e-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="f3f2e-160">correlationId</span></span>|<span data-ttu-id="f3f2e-161">Guid</span><span class="sxs-lookup"><span data-stu-id="f3f2e-161">Guid</span></span>|<span data-ttu-id="f3f2e-162">A ID da solicitação de cliente usada para correlacionar a atividade dentro do sistema.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="f3f2e-163">recursos</span><span class="sxs-lookup"><span data-stu-id="f3f2e-163">resources</span></span>|<span data-ttu-id="f3f2e-164">Coleção [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="f3f2e-164">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="f3f2e-165">Recursos em modificação.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-165">Resources being modified.</span></span>|
|<span data-ttu-id="f3f2e-166">category</span><span class="sxs-lookup"><span data-stu-id="f3f2e-166">category</span></span>|<span data-ttu-id="f3f2e-167">String</span><span class="sxs-lookup"><span data-stu-id="f3f2e-167">String</span></span>|<span data-ttu-id="f3f2e-168">Categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-168">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="f3f2e-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3f2e-169">Response</span></span>
<span data-ttu-id="f3f2e-170">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [auditEvent](../resources/intune-auditing-auditevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-170">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3f2e-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f3f2e-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3f2e-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f3f2e-172">Request</span></span>
<span data-ttu-id="f3f2e-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f3f2e-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="f3f2e-174">Response</span></span>
<span data-ttu-id="f3f2e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f3f2e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





