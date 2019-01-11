---
title: função getRoleScopeTagsByResource
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 736c1d8c874d0eb5ae2ce42ac9b9f17a98554879
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890556"
---
# <a name="getrolescopetagsbyresource-function"></a><span data-ttu-id="9f073-103">função getRoleScopeTagsByResource</span><span class="sxs-lookup"><span data-stu-id="9f073-103">getRoleScopeTagsByResource function</span></span>

> <span data-ttu-id="9f073-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9f073-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f073-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9f073-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f073-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9f073-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f073-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9f073-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f073-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9f073-108">Prerequisites</span></span>
<span data-ttu-id="9f073-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f073-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f073-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f073-111">Permission type</span></span>|<span data-ttu-id="9f073-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9f073-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f073-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f073-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9f073-114">&nbsp;&nbsp; **O controle de acesso baseado em função (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="9f073-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="9f073-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="9f073-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="9f073-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f073-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f073-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f073-117">Not supported.</span></span>|
|<span data-ttu-id="9f073-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f073-118">Application</span></span>|<span data-ttu-id="9f073-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f073-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f073-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f073-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getRoleScopeTagsByResource
```

## <a name="request-headers"></a><span data-ttu-id="9f073-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9f073-121">Request headers</span></span>
|<span data-ttu-id="9f073-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9f073-122">Header</span></span>|<span data-ttu-id="9f073-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9f073-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f073-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9f073-124">Authorization</span></span>|<span data-ttu-id="9f073-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9f073-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f073-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9f073-126">Accept</span></span>|<span data-ttu-id="9f073-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9f073-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f073-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f073-128">Request body</span></span>
<span data-ttu-id="9f073-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="9f073-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9f073-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="9f073-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9f073-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f073-131">Property</span></span>|<span data-ttu-id="9f073-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f073-132">Type</span></span>|<span data-ttu-id="9f073-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f073-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f073-134">recurso</span><span class="sxs-lookup"><span data-stu-id="9f073-134">resource</span></span>|<span data-ttu-id="9f073-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f073-135">String</span></span>|<span data-ttu-id="9f073-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9f073-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9f073-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f073-137">Response</span></span>
<span data-ttu-id="9f073-138">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um conjunto de [roleScopeTag](../resources/intune-rbac-rolescopetag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9f073-138">If successful, this function returns a `200 OK` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f073-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9f073-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f073-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9f073-140">Request</span></span>
<span data-ttu-id="9f073-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9f073-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getRoleScopeTagsByResource(resource='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9f073-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f073-142">Response</span></span>
<span data-ttu-id="9f073-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9f073-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



