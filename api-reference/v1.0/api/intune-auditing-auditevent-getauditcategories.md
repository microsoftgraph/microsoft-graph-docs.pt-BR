---
title: Função getAuditCategories
description: Ainda não documentado
ms.openlocfilehash: 4e54768c6381f947ea9b65751986f756422a46fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006796"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="94af8-103">Função getAuditCategories</span><span class="sxs-lookup"><span data-stu-id="94af8-103">getAuditCategories function</span></span>

> <span data-ttu-id="94af8-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="94af8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94af8-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="94af8-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94af8-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94af8-106">Prerequisites</span></span>
<span data-ttu-id="94af8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94af8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94af8-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94af8-109">Permission type</span></span>|<span data-ttu-id="94af8-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94af8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94af8-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94af8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="94af8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="94af8-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="94af8-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94af8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94af8-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94af8-114">Not supported.</span></span>|
|<span data-ttu-id="94af8-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94af8-115">Application</span></span>|<span data-ttu-id="94af8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94af8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94af8-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94af8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="94af8-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94af8-118">Request headers</span></span>
|<span data-ttu-id="94af8-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94af8-119">Header</span></span>|<span data-ttu-id="94af8-120">Valor</span><span class="sxs-lookup"><span data-stu-id="94af8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94af8-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="94af8-121">Authorization</span></span>|<span data-ttu-id="94af8-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94af8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94af8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="94af8-123">Accept</span></span>|<span data-ttu-id="94af8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="94af8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94af8-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94af8-125">Request body</span></span>
<span data-ttu-id="94af8-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="94af8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94af8-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="94af8-127">Response</span></span>
<span data-ttu-id="94af8-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94af8-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94af8-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94af8-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="94af8-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94af8-130">Request</span></span>
<span data-ttu-id="94af8-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94af8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="94af8-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="94af8-132">Response</span></span>
<span data-ttu-id="94af8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94af8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": [
    "Get Audit Categories value"
  ]
}
```



