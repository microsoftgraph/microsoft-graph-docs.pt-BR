---
title: função getRoleScopeTagsByResource
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a578b68c0756a86d31ddc3ded8036a3b095b5a0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725833"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="903b1-103">função getRoleScopeTagsByResource</span><span class="sxs-lookup"><span data-stu-id="903b1-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="903b1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="903b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="903b1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="903b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="903b1-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="903b1-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="903b1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="903b1-107">Prerequisites</span></span>
<span data-ttu-id="903b1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="903b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="903b1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="903b1-110">Permission type</span></span>|<span data-ttu-id="903b1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="903b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="903b1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="903b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="903b1-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="903b1-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="903b1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="903b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="903b1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="903b1-115">Not supported.</span></span>|
|<span data-ttu-id="903b1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="903b1-116">Application</span></span>|<span data-ttu-id="903b1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="903b1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="903b1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="903b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="903b1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="903b1-119">Request headers</span></span>
|<span data-ttu-id="903b1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="903b1-120">Header</span></span>|<span data-ttu-id="903b1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="903b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="903b1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="903b1-122">Authorization</span></span>|<span data-ttu-id="903b1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="903b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="903b1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="903b1-124">Accept</span></span>|<span data-ttu-id="903b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="903b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="903b1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="903b1-126">Request body</span></span>
<span data-ttu-id="903b1-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="903b1-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="903b1-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="903b1-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="903b1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="903b1-129">Property</span></span>|<span data-ttu-id="903b1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="903b1-130">Type</span></span>|<span data-ttu-id="903b1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="903b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="903b1-132">recurso</span><span class="sxs-lookup"><span data-stu-id="903b1-132">resource</span></span>|<span data-ttu-id="903b1-133">String</span><span class="sxs-lookup"><span data-stu-id="903b1-133">String</span></span>|<span data-ttu-id="903b1-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="903b1-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="903b1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="903b1-135">Response</span></span>
<span data-ttu-id="903b1-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="903b1-136">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="903b1-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="903b1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="903b1-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="903b1-138">Request</span></span>
<span data-ttu-id="903b1-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="903b1-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="903b1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="903b1-140">Response</span></span>
<span data-ttu-id="903b1-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="903b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTag",
      "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```





