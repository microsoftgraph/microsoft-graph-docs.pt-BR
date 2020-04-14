---
title: Obter roleScopeTag
description: Leia as propriedades e as relações do objeto roleScopeTag.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f789f363811648a75743d1133ae09977d94d3540
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463604"
---
# <a name="get-rolescopetag"></a><span data-ttu-id="09c55-103">Obter roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="09c55-103">Get roleScopeTag</span></span>

<span data-ttu-id="09c55-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09c55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09c55-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09c55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09c55-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09c55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09c55-107">Leia as propriedades e as relações do objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="09c55-107">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09c55-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="09c55-108">Prerequisites</span></span>
<span data-ttu-id="09c55-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09c55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09c55-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09c55-111">Permission type</span></span>|<span data-ttu-id="09c55-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="09c55-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09c55-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09c55-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09c55-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="09c55-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="09c55-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09c55-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09c55-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09c55-116">Not supported.</span></span>|
|<span data-ttu-id="09c55-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09c55-117">Application</span></span>|<span data-ttu-id="09c55-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="09c55-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="09c55-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09c55-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags/{roleScopeTagId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09c55-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="09c55-120">Optional query parameters</span></span>
<span data-ttu-id="09c55-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="09c55-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09c55-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09c55-122">Request headers</span></span>
|<span data-ttu-id="09c55-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="09c55-123">Header</span></span>|<span data-ttu-id="09c55-124">Valor</span><span class="sxs-lookup"><span data-stu-id="09c55-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09c55-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="09c55-125">Authorization</span></span>|<span data-ttu-id="09c55-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09c55-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09c55-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="09c55-127">Accept</span></span>|<span data-ttu-id="09c55-128">application/json</span><span class="sxs-lookup"><span data-stu-id="09c55-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09c55-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09c55-129">Request body</span></span>
<span data-ttu-id="09c55-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09c55-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09c55-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="09c55-131">Response</span></span>
<span data-ttu-id="09c55-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09c55-132">If successful, this method returns a `200 OK` response code and [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09c55-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09c55-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="09c55-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09c55-134">Request</span></span>
<span data-ttu-id="09c55-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="09c55-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
```

### <a name="response"></a><span data-ttu-id="09c55-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="09c55-136">Response</span></span>
<span data-ttu-id="09c55-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09c55-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": {
    "@odata.type": "#microsoft.graph.roleScopeTag",
    "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
    "displayName": "Display Name value",
    "description": "Description value",
    "isBuiltIn": true
  }
}
```



