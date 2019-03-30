---
title: Obter roleScopeTag
description: Leia as propriedades e as relações do objeto roleScopeTag.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: afa9eefdb11db4b2881c100691a3876a9dd96861
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985785"
---
# <a name="get-rolescopetag"></a><span data-ttu-id="9ff35-103">Obter roleScopeTag</span><span class="sxs-lookup"><span data-stu-id="9ff35-103">Get roleScopeTag</span></span>

> <span data-ttu-id="9ff35-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ff35-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ff35-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ff35-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ff35-106">Leia as propriedades e as relações do objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="9ff35-106">Read properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ff35-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ff35-107">Prerequisites</span></span>
<span data-ttu-id="9ff35-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ff35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ff35-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ff35-110">Permission type</span></span>|<span data-ttu-id="9ff35-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ff35-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ff35-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ff35-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ff35-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ff35-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="9ff35-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ff35-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ff35-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ff35-115">Not supported.</span></span>|
|<span data-ttu-id="9ff35-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ff35-116">Application</span></span>|<span data-ttu-id="9ff35-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ff35-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ff35-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ff35-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags/{roleScopeTagId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ff35-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ff35-119">Optional query parameters</span></span>
<span data-ttu-id="9ff35-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ff35-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ff35-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff35-121">Request headers</span></span>
|<span data-ttu-id="9ff35-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ff35-122">Header</span></span>|<span data-ttu-id="9ff35-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9ff35-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ff35-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ff35-124">Authorization</span></span>|<span data-ttu-id="9ff35-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ff35-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ff35-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ff35-126">Accept</span></span>|<span data-ttu-id="9ff35-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9ff35-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ff35-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff35-128">Request body</span></span>
<span data-ttu-id="9ff35-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ff35-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ff35-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ff35-130">Response</span></span>
<span data-ttu-id="9ff35-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ff35-131">If successful, this method returns a `200 OK` response code and [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ff35-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ff35-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ff35-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ff35-133">Request</span></span>
<span data-ttu-id="9ff35-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ff35-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
```

### <a name="response"></a><span data-ttu-id="9ff35-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ff35-135">Response</span></span>
<span data-ttu-id="9ff35-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ff35-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 209

{
  "value": {
    "@odata.type": "#microsoft.graph.roleScopeTag",
    "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```




