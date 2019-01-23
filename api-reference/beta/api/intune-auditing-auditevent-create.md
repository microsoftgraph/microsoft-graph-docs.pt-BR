---
title: Criar auditEvent
description: Criar um novo objeto auditEvent.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6f7a8bac0030b65d61e1da7fbdadfe6920b44788
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422149"
---
# <a name="create-auditevent"></a><span data-ttu-id="e6dad-103">Criar auditEvent</span><span class="sxs-lookup"><span data-stu-id="e6dad-103">Create auditEvent</span></span>

> <span data-ttu-id="e6dad-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e6dad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e6dad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e6dad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6dad-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e6dad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6dad-107">Criar um novo objeto [auditEvent](../resources/intune-auditing-auditevent.md).</span><span class="sxs-lookup"><span data-stu-id="e6dad-107">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e6dad-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e6dad-108">Prerequisites</span></span>
<span data-ttu-id="e6dad-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e6dad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e6dad-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e6dad-111">Permission type</span></span>|<span data-ttu-id="e6dad-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e6dad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6dad-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e6dad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e6dad-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6dad-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e6dad-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e6dad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6dad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6dad-116">Not supported.</span></span>|
|<span data-ttu-id="e6dad-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e6dad-117">Application</span></span>|<span data-ttu-id="e6dad-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e6dad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6dad-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e6dad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="e6dad-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e6dad-120">Request headers</span></span>
|<span data-ttu-id="e6dad-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e6dad-121">Header</span></span>|<span data-ttu-id="e6dad-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e6dad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6dad-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e6dad-123">Authorization</span></span>|<span data-ttu-id="e6dad-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e6dad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e6dad-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e6dad-125">Accept</span></span>|<span data-ttu-id="e6dad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6dad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6dad-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e6dad-127">Request body</span></span>
<span data-ttu-id="e6dad-128">No corpo da solicitação, forneça uma representação JSON do objeto auditEvent.</span><span class="sxs-lookup"><span data-stu-id="e6dad-128">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="e6dad-129">A tabela a seguir mostra as propriedades que são necessárias ao criar auditEvent.</span><span class="sxs-lookup"><span data-stu-id="e6dad-129">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="e6dad-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6dad-130">Property</span></span>|<span data-ttu-id="e6dad-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6dad-131">Type</span></span>|<span data-ttu-id="e6dad-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6dad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6dad-133">id</span><span class="sxs-lookup"><span data-stu-id="e6dad-133">id</span></span>|<span data-ttu-id="e6dad-134">String</span><span class="sxs-lookup"><span data-stu-id="e6dad-134">String</span></span>|<span data-ttu-id="e6dad-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e6dad-135">Key of the entity.</span></span>|
|<span data-ttu-id="e6dad-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e6dad-136">displayName</span></span>|<span data-ttu-id="e6dad-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6dad-137">String</span></span>|<span data-ttu-id="e6dad-138">Nome de exibição do evento.</span><span class="sxs-lookup"><span data-stu-id="e6dad-138">Event display name.</span></span>|
|<span data-ttu-id="e6dad-139">componentName</span><span class="sxs-lookup"><span data-stu-id="e6dad-139">componentName</span></span>|<span data-ttu-id="e6dad-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6dad-140">String</span></span>|<span data-ttu-id="e6dad-141">Nome do componente.</span><span class="sxs-lookup"><span data-stu-id="e6dad-141">Component name.</span></span>|
|<span data-ttu-id="e6dad-142">actor</span><span class="sxs-lookup"><span data-stu-id="e6dad-142">actor</span></span>|[<span data-ttu-id="e6dad-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="e6dad-143">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="e6dad-144">Usuários e aplicativos do AAD associados com o evento de auditoria.</span><span class="sxs-lookup"><span data-stu-id="e6dad-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="e6dad-145">atividade</span><span class="sxs-lookup"><span data-stu-id="e6dad-145">activity</span></span>|<span data-ttu-id="e6dad-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6dad-146">String</span></span>|<span data-ttu-id="e6dad-147">Nome amigável da atividade.</span><span class="sxs-lookup"><span data-stu-id="e6dad-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="e6dad-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="e6dad-148">activityDateTime</span></span>|<span data-ttu-id="e6dad-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6dad-149">DateTimeOffset</span></span>|<span data-ttu-id="e6dad-150">A hora e data em UTC em que a atividade foi executada.</span><span class="sxs-lookup"><span data-stu-id="e6dad-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="e6dad-151">activityType</span><span class="sxs-lookup"><span data-stu-id="e6dad-151">activityType</span></span>|<span data-ttu-id="e6dad-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6dad-152">String</span></span>|<span data-ttu-id="e6dad-153">O tipo de atividade que foi executada.</span><span class="sxs-lookup"><span data-stu-id="e6dad-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="e6dad-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="e6dad-154">activityOperationType</span></span>|<span data-ttu-id="e6dad-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6dad-155">String</span></span>|<span data-ttu-id="e6dad-156">O tipo de operação HTTP da atividade.</span><span class="sxs-lookup"><span data-stu-id="e6dad-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="e6dad-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="e6dad-157">activityResult</span></span>|<span data-ttu-id="e6dad-158">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6dad-158">String</span></span>|<span data-ttu-id="e6dad-159">O resultado da atividade.</span><span class="sxs-lookup"><span data-stu-id="e6dad-159">The result of the activity.</span></span>|
|<span data-ttu-id="e6dad-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="e6dad-160">correlationId</span></span>|<span data-ttu-id="e6dad-161">Guid</span><span class="sxs-lookup"><span data-stu-id="e6dad-161">Guid</span></span>|<span data-ttu-id="e6dad-162">A ID da solicitação de cliente usada para correlacionar a atividade dentro do sistema.</span><span class="sxs-lookup"><span data-stu-id="e6dad-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="e6dad-163">recursos</span><span class="sxs-lookup"><span data-stu-id="e6dad-163">resources</span></span>|<span data-ttu-id="e6dad-164">Coleção [auditResource](../resources/intune-auditing-auditresource.md)</span><span class="sxs-lookup"><span data-stu-id="e6dad-164">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="e6dad-165">Recursos em modificação.</span><span class="sxs-lookup"><span data-stu-id="e6dad-165">Resources being modified.</span></span>|
|<span data-ttu-id="e6dad-166">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="e6dad-166">category</span></span>|<span data-ttu-id="e6dad-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6dad-167">String</span></span>|<span data-ttu-id="e6dad-168">Categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="e6dad-168">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="e6dad-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6dad-169">Response</span></span>
<span data-ttu-id="e6dad-170">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [auditEvent](../resources/intune-auditing-auditevent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e6dad-170">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6dad-171">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e6dad-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="e6dad-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e6dad-172">Request</span></span>
<span data-ttu-id="e6dad-173">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e6dad-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
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

### <a name="response"></a><span data-ttu-id="e6dad-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="e6dad-174">Response</span></span>
<span data-ttu-id="e6dad-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e6dad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




