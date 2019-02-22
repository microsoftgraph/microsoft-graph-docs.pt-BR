---
title: função getRoleScopeTagsByResource
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 54cc2ba137a3c4a45fc3ca724fa47c1f3f3e0490
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140660"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="4f876-103">função getRoleScopeTagsByResource</span><span class="sxs-lookup"><span data-stu-id="4f876-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="4f876-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4f876-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4f876-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4f876-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f876-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f876-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f876-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4f876-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f876-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f876-108">Prerequisites</span></span>
<span data-ttu-id="4f876-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f876-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="4f876-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f876-111">Permission type</span></span>|<span data-ttu-id="4f876-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f876-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f876-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f876-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4f876-114">&nbsp;&nbsp; **Controle de acesso baseado em função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="4f876-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="4f876-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="4f876-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="4f876-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f876-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f876-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f876-117">Not supported.</span></span>|
|<span data-ttu-id="4f876-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4f876-118">Application</span></span>|<span data-ttu-id="4f876-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f876-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f876-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f876-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="4f876-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f876-121">Request headers</span></span>
|<span data-ttu-id="4f876-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f876-122">Header</span></span>|<span data-ttu-id="4f876-123">Valor</span><span class="sxs-lookup"><span data-stu-id="4f876-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f876-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f876-124">Authorization</span></span>|<span data-ttu-id="4f876-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f876-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f876-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f876-126">Accept</span></span>|<span data-ttu-id="4f876-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4f876-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f876-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f876-128">Request body</span></span>
<span data-ttu-id="4f876-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="4f876-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4f876-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="4f876-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4f876-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f876-131">Property</span></span>|<span data-ttu-id="4f876-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f876-132">Type</span></span>|<span data-ttu-id="4f876-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f876-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f876-134">recurso</span><span class="sxs-lookup"><span data-stu-id="4f876-134">resource</span></span>|<span data-ttu-id="4f876-135">String</span><span class="sxs-lookup"><span data-stu-id="4f876-135">String</span></span>|<span data-ttu-id="4f876-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4f876-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4f876-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f876-137">Response</span></span>
<span data-ttu-id="4f876-138">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f876-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f876-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f876-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f876-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f876-140">Request</span></span>
<span data-ttu-id="4f876-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f876-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4f876-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f876-142">Response</span></span>
<span data-ttu-id="4f876-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f876-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



