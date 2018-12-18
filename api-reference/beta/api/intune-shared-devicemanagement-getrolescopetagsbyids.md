---
title: função getRoleScopeTagsByIds
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: b6708a605ad0c528e691b0a9a3a218e178ff7730
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342487"
---
# <a name="getrolescopetagsbyids-function"></a><span data-ttu-id="99b7d-103">função getRoleScopeTagsByIds</span><span class="sxs-lookup"><span data-stu-id="99b7d-103">getRoleScopeTagsByIds function</span></span>

> <span data-ttu-id="99b7d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99b7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99b7d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99b7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99b7d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="99b7d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99b7d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="99b7d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99b7d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99b7d-108">Prerequisites</span></span>
<span data-ttu-id="99b7d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99b7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99b7d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99b7d-111">Permission type</span></span>|<span data-ttu-id="99b7d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99b7d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99b7d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99b7d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="99b7d-114">&nbsp;&nbsp; **O controle de acesso baseado em função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="99b7d-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="99b7d-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="99b7d-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="99b7d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99b7d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99b7d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99b7d-117">Not supported.</span></span>|
|<span data-ttu-id="99b7d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99b7d-118">Application</span></span>|<span data-ttu-id="99b7d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99b7d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99b7d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99b7d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByIds
```

## <a name="request-headers"></a><span data-ttu-id="99b7d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99b7d-121">Request headers</span></span>
|<span data-ttu-id="99b7d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99b7d-122">Header</span></span>|<span data-ttu-id="99b7d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="99b7d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99b7d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="99b7d-124">Authorization</span></span>|<span data-ttu-id="99b7d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99b7d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99b7d-126">Accept</span><span class="sxs-lookup"><span data-stu-id="99b7d-126">Accept</span></span>|<span data-ttu-id="99b7d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="99b7d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99b7d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99b7d-128">Request body</span></span>
<span data-ttu-id="99b7d-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="99b7d-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="99b7d-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="99b7d-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="99b7d-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99b7d-131">Property</span></span>|<span data-ttu-id="99b7d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="99b7d-132">Type</span></span>|<span data-ttu-id="99b7d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="99b7d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99b7d-134">ids</span><span class="sxs-lookup"><span data-stu-id="99b7d-134">ids</span></span>|<span data-ttu-id="99b7d-135">String collection</span><span class="sxs-lookup"><span data-stu-id="99b7d-135">String collection</span></span>|<span data-ttu-id="99b7d-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="99b7d-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="99b7d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="99b7d-137">Response</span></span>
<span data-ttu-id="99b7d-138">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um conjunto de [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99b7d-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99b7d-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99b7d-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="99b7d-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99b7d-140">Request</span></span>
<span data-ttu-id="99b7d-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99b7d-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByIds(ids=[
  "Ids value"
])
```

### <a name="response"></a><span data-ttu-id="99b7d-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="99b7d-142">Response</span></span>
<span data-ttu-id="99b7d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99b7d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



