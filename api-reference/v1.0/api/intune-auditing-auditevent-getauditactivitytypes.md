---
title: Função getAuditActivityTypes
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3a8151169f1173594be3697e721e89556416e718
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952675"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="a69c5-103">Função getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="a69c5-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="a69c5-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a69c5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a69c5-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a69c5-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a69c5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a69c5-106">Prerequisites</span></span>
<span data-ttu-id="a69c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a69c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a69c5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a69c5-109">Permission type</span></span>|<span data-ttu-id="a69c5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a69c5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a69c5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a69c5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a69c5-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a69c5-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a69c5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a69c5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a69c5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a69c5-114">Not supported.</span></span>|
|<span data-ttu-id="a69c5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a69c5-115">Application</span></span>|<span data-ttu-id="a69c5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a69c5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a69c5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a69c5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="a69c5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a69c5-118">Request headers</span></span>
|<span data-ttu-id="a69c5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a69c5-119">Header</span></span>|<span data-ttu-id="a69c5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="a69c5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a69c5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a69c5-121">Authorization</span></span>|<span data-ttu-id="a69c5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a69c5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a69c5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a69c5-123">Accept</span></span>|<span data-ttu-id="a69c5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a69c5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a69c5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a69c5-125">Request body</span></span>
<span data-ttu-id="a69c5-126">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="a69c5-126">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a69c5-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="a69c5-127">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a69c5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a69c5-128">Property</span></span>|<span data-ttu-id="a69c5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="a69c5-129">Type</span></span>|<span data-ttu-id="a69c5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a69c5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a69c5-131">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="a69c5-131">category</span></span>|<span data-ttu-id="a69c5-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a69c5-132">String</span></span>|<span data-ttu-id="a69c5-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a69c5-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a69c5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a69c5-134">Response</span></span>
<span data-ttu-id="a69c5-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a69c5-135">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a69c5-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a69c5-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="a69c5-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a69c5-137">Request</span></span>
<span data-ttu-id="a69c5-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a69c5-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a69c5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a69c5-139">Response</span></span>
<span data-ttu-id="a69c5-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a69c5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 61

{
  "value": [
    "Get Audit Activity Types value"
  ]
}
```



