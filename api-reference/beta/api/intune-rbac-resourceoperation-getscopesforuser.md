---
title: função getScopesForUser
description: Ainda não documentado
ms.openlocfilehash: 0cd39dec7cb90623981ee6be1a6c6ad96002d0e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037901"
---
# <a name="getscopesforuser-function"></a><span data-ttu-id="b7a4d-103">função getScopesForUser</span><span class="sxs-lookup"><span data-stu-id="b7a4d-103">getScopesForUser function</span></span>

> <span data-ttu-id="b7a4d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7a4d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7a4d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7a4d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b7a4d-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b7a4d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7a4d-108">Prerequisites</span></span>
<span data-ttu-id="b7a4d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7a4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7a4d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7a4d-111">Permission type</span></span>|<span data-ttu-id="b7a4d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b7a4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7a4d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7a4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7a4d-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7a4d-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="b7a4d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7a4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7a4d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-116">Not supported.</span></span>|
|<span data-ttu-id="b7a4d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7a4d-117">Application</span></span>|<span data-ttu-id="b7a4d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7a4d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7a4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser
```

## <a name="request-headers"></a><span data-ttu-id="b7a4d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a4d-120">Request headers</span></span>
|<span data-ttu-id="b7a4d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7a4d-121">Header</span></span>|<span data-ttu-id="b7a4d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b7a4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7a4d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7a4d-123">Authorization</span></span>|<span data-ttu-id="b7a4d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7a4d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b7a4d-125">Accept</span></span>|<span data-ttu-id="b7a4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7a4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7a4d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a4d-127">Request body</span></span>
<span data-ttu-id="b7a4d-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b7a4d-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b7a4d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7a4d-130">Property</span></span>|<span data-ttu-id="b7a4d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7a4d-131">Type</span></span>|<span data-ttu-id="b7a4d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7a4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7a4d-133">UserID</span><span class="sxs-lookup"><span data-stu-id="b7a4d-133">userid</span></span>|<span data-ttu-id="b7a4d-134">String</span><span class="sxs-lookup"><span data-stu-id="b7a4d-134">String</span></span>|<span data-ttu-id="b7a4d-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b7a4d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b7a4d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7a4d-136">Response</span></span>
<span data-ttu-id="b7a4d-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7a4d-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7a4d-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="b7a4d-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7a4d-139">Request</span></span>
<span data-ttu-id="b7a4d-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}/getScopesForUser(userid='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b7a4d-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7a4d-141">Response</span></span>
<span data-ttu-id="b7a4d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7a4d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 56

{
  "value": [
    "Get Scopes For User value"
  ]
}
```





