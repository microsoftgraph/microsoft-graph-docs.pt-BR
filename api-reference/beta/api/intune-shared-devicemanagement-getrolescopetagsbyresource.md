---
title: função getRoleScopeTagsByResource
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b8e59c2179562c1c3e605307f5aa6ab0dd54cb6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706328"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="2f74f-103">função getRoleScopeTagsByResource</span><span class="sxs-lookup"><span data-stu-id="2f74f-103">getRoleScopeTagsByResource function</span></span>

<span data-ttu-id="2f74f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f74f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f74f-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2f74f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2f74f-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2f74f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2f74f-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f74f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f74f-108">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2f74f-108">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2f74f-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f74f-109">Prerequisites</span></span>
<span data-ttu-id="2f74f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f74f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f74f-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f74f-112">Permission type</span></span>|<span data-ttu-id="2f74f-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f74f-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f74f-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f74f-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2f74f-115">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="2f74f-115">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="2f74f-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f74f-116">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="2f74f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f74f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f74f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f74f-118">Not supported.</span></span>|
|<span data-ttu-id="2f74f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f74f-119">Application</span></span>||
| <span data-ttu-id="2f74f-120">&nbsp; &nbsp; **Controle de Acesso Baseado em Função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="2f74f-120">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="2f74f-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="2f74f-121">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f74f-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f74f-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="2f74f-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f74f-123">Request headers</span></span>
|<span data-ttu-id="2f74f-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f74f-124">Header</span></span>|<span data-ttu-id="2f74f-125">Valor</span><span class="sxs-lookup"><span data-stu-id="2f74f-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f74f-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f74f-126">Authorization</span></span>|<span data-ttu-id="2f74f-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f74f-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f74f-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f74f-128">Accept</span></span>|<span data-ttu-id="2f74f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="2f74f-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f74f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f74f-130">Request body</span></span>
<span data-ttu-id="2f74f-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="2f74f-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2f74f-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="2f74f-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2f74f-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f74f-133">Property</span></span>|<span data-ttu-id="2f74f-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f74f-134">Type</span></span>|<span data-ttu-id="2f74f-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f74f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f74f-136">recurso</span><span class="sxs-lookup"><span data-stu-id="2f74f-136">resource</span></span>|<span data-ttu-id="2f74f-137">String</span><span class="sxs-lookup"><span data-stu-id="2f74f-137">String</span></span>|<span data-ttu-id="2f74f-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2f74f-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2f74f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f74f-139">Response</span></span>
<span data-ttu-id="2f74f-140">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f74f-140">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f74f-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f74f-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="2f74f-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f74f-142">Request</span></span>
<span data-ttu-id="2f74f-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f74f-143">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2f74f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f74f-144">Response</span></span>
<span data-ttu-id="2f74f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f74f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











