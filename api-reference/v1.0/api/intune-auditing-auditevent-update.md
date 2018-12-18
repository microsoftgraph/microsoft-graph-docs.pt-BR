---
title: Atualizar auditEvent
description: Atualizar as propriedades do objeto auditEvent.
author: tfitzmac
ms.openlocfilehash: 631144a0192af20580cdbf108d3acf7daa3d82f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310042"
---
# <a name="update-auditevent"></a><span data-ttu-id="bbba4-103">Atualizar auditEvent</span><span class="sxs-lookup"><span data-stu-id="bbba4-103">Update auditEvent</span></span>

> <span data-ttu-id="bbba4-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bbba4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbba4-105">Atualizar as propriedades do objeto [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="bbba4-105">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbba4-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bbba4-106">Prerequisites</span></span>
<span data-ttu-id="bbba4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bbba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bbba4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bbba4-109">Permission type</span></span>|<span data-ttu-id="bbba4-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bbba4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbba4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bbba4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bbba4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbba4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bbba4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bbba4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbba4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbba4-114">Not supported.</span></span>|
|<span data-ttu-id="bbba4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bbba4-115">Application</span></span>|<span data-ttu-id="bbba4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bbba4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbba4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bbba4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="bbba4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bbba4-118">Request headers</span></span>
|<span data-ttu-id="bbba4-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bbba4-119">Header</span></span>|<span data-ttu-id="bbba4-120">Valor</span><span class="sxs-lookup"><span data-stu-id="bbba4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbba4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bbba4-121">Authorization</span></span>|<span data-ttu-id="bbba4-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bbba4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbba4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bbba4-123">Accept</span></span>|<span data-ttu-id="bbba4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bbba4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbba4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bbba4-125">Request body</span></span>
<span data-ttu-id="bbba4-126">No corpo da solicitação, forneça uma representação JSON do objeto [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="bbba4-126">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="bbba4-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="bbba4-127">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="bbba4-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbba4-128">Property</span></span>|<span data-ttu-id="bbba4-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbba4-129">Type</span></span>|<span data-ttu-id="bbba4-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbba4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbba4-131">id</span><span class="sxs-lookup"><span data-stu-id="bbba4-131">id</span></span>|<span data-ttu-id="bbba4-132">String</span><span class="sxs-lookup"><span data-stu-id="bbba4-132">String</span></span>|<span data-ttu-id="bbba4-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bbba4-133">Key of the entity.</span></span>|
|<span data-ttu-id="bbba4-134">displayName</span><span class="sxs-lookup"><span data-stu-id="bbba4-134">displayName</span></span>|<span data-ttu-id="bbba4-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbba4-135">String</span></span>|<span data-ttu-id="bbba4-136">Nome de exibição do evento.</span><span class="sxs-lookup"><span data-stu-id="bbba4-136">Event display name.</span></span>|
|<span data-ttu-id="bbba4-137">componentName</span><span class="sxs-lookup"><span data-stu-id="bbba4-137">componentName</span></span>|<span data-ttu-id="bbba4-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbba4-138">String</span></span>|<span data-ttu-id="bbba4-139">Nome do componente.</span><span class="sxs-lookup"><span data-stu-id="bbba4-139">Component name.</span></span>|
|<span data-ttu-id="bbba4-140">actor</span><span class="sxs-lookup"><span data-stu-id="bbba4-140">actor</span></span>|[<span data-ttu-id="bbba4-141">auditActor</span><span class="sxs-lookup"><span data-stu-id="bbba4-141">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="bbba4-142">Usuários e aplicativos do AAD associados com o evento de auditoria.</span><span class="sxs-lookup"><span data-stu-id="bbba4-142">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="bbba4-143">atividade</span><span class="sxs-lookup"><span data-stu-id="bbba4-143">activity</span></span>|<span data-ttu-id="bbba4-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbba4-144">String</span></span>|<span data-ttu-id="bbba4-145">Nome amigável da atividade.</span><span class="sxs-lookup"><span data-stu-id="bbba4-145">Friendly name of the activity.</span></span>|
|<span data-ttu-id="bbba4-146">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="bbba4-146">activityDateTime</span></span>|<span data-ttu-id="bbba4-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbba4-147">DateTimeOffset</span></span>|<span data-ttu-id="bbba4-148">A hora e data em UTC em que a atividade foi executada.</span><span class="sxs-lookup"><span data-stu-id="bbba4-148">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="bbba4-149">activityType</span><span class="sxs-lookup"><span data-stu-id="bbba4-149">activityType</span></span>|<span data-ttu-id="bbba4-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbba4-150">String</span></span>|<span data-ttu-id="bbba4-151">O tipo de atividade que foi executada.</span><span class="sxs-lookup"><span data-stu-id="bbba4-151">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="bbba4-152">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="bbba4-152">activityOperationType</span></span>|<span data-ttu-id="bbba4-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbba4-153">String</span></span>|<span data-ttu-id="bbba4-154">O tipo de operação HTTP da atividade.</span><span class="sxs-lookup"><span data-stu-id="bbba4-154">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="bbba4-155">activityResult</span><span class="sxs-lookup"><span data-stu-id="bbba4-155">activityResult</span></span>|<span data-ttu-id="bbba4-156">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbba4-156">String</span></span>|<span data-ttu-id="bbba4-157">O resultado da atividade.</span><span class="sxs-lookup"><span data-stu-id="bbba4-157">The result of the activity.</span></span>|
|<span data-ttu-id="bbba4-158">correlationId</span><span class="sxs-lookup"><span data-stu-id="bbba4-158">correlationId</span></span>|<span data-ttu-id="bbba4-159">Guid</span><span class="sxs-lookup"><span data-stu-id="bbba4-159">Guid</span></span>|<span data-ttu-id="bbba4-160">A ID da solicitação de cliente usada para correlacionar a atividade dentro do sistema.</span><span class="sxs-lookup"><span data-stu-id="bbba4-160">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="bbba4-161">recursos</span><span class="sxs-lookup"><span data-stu-id="bbba4-161">resources</span></span>|<span data-ttu-id="bbba4-162">Coleção [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="bbba4-162">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="bbba4-163">Recursos em modificação.</span><span class="sxs-lookup"><span data-stu-id="bbba4-163">Resources being modified.</span></span>|
|<span data-ttu-id="bbba4-164">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="bbba4-164">category</span></span>|<span data-ttu-id="bbba4-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbba4-165">String</span></span>|<span data-ttu-id="bbba4-166">Categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="bbba4-166">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="bbba4-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbba4-167">Response</span></span>
<span data-ttu-id="bbba4-168">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [auditEvent](../resources/intune-auditing-auditevent.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bbba4-168">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbba4-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bbba4-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbba4-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bbba4-170">Request</span></span>
<span data-ttu-id="bbba4-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bbba4-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
Content-type: application/json
Content-length: 1390

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
    "userId": "User Id value"
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

### <a name="response"></a><span data-ttu-id="bbba4-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="bbba4-172">Response</span></span>
<span data-ttu-id="bbba4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bbba4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

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
    "userId": "User Id value"
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



