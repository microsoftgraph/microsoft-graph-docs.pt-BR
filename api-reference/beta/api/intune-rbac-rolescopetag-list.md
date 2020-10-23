---
title: Listar roleScopeTags
description: Listar Propriedades e relações dos objetos roleScopeTag.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02a200e3ce9ded6bb9cb545eb4dacf794e9ad877
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703955"
---
# <a name="list-rolescopetags"></a><span data-ttu-id="631fc-103">Listar roleScopeTags</span><span class="sxs-lookup"><span data-stu-id="631fc-103">List roleScopeTags</span></span>

<span data-ttu-id="631fc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="631fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="631fc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="631fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="631fc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="631fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="631fc-107">Listar Propriedades e relações dos objetos [roleScopeTag](../resources/intune-rbac-rolescopetag.md) .</span><span class="sxs-lookup"><span data-stu-id="631fc-107">List properties and relationships of the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="631fc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="631fc-108">Prerequisites</span></span>
<span data-ttu-id="631fc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="631fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="631fc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="631fc-111">Permission type</span></span>|<span data-ttu-id="631fc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="631fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="631fc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="631fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="631fc-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="631fc-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="631fc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="631fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="631fc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="631fc-116">Not supported.</span></span>|
|<span data-ttu-id="631fc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="631fc-117">Application</span></span>|<span data-ttu-id="631fc-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="631fc-118">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="631fc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="631fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="631fc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="631fc-120">Request headers</span></span>
|<span data-ttu-id="631fc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="631fc-121">Header</span></span>|<span data-ttu-id="631fc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="631fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="631fc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="631fc-123">Authorization</span></span>|<span data-ttu-id="631fc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="631fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="631fc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="631fc-125">Accept</span></span>|<span data-ttu-id="631fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="631fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="631fc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="631fc-127">Request body</span></span>
<span data-ttu-id="631fc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="631fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="631fc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="631fc-129">Response</span></span>
<span data-ttu-id="631fc-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="631fc-130">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTag](../resources/intune-rbac-rolescopetag.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="631fc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="631fc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="631fc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="631fc-132">Request</span></span>
<span data-ttu-id="631fc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="631fc-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
```

### <a name="response"></a><span data-ttu-id="631fc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="631fc-134">Response</span></span>
<span data-ttu-id="631fc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="631fc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value",
      "isBuiltIn": true
    }
  ]
}
```





