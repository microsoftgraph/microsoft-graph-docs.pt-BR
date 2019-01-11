---
title: Função getAuditActivityTypes
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a0a8087b1a1bb61fcbd414da7d1f72bb33caccf9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823096"
---
# <a name="getauditactivitytypes-function"></a><span data-ttu-id="b9df0-103">Função getAuditActivityTypes</span><span class="sxs-lookup"><span data-stu-id="b9df0-103">getAuditActivityTypes function</span></span>

> <span data-ttu-id="b9df0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b9df0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9df0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b9df0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b9df0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b9df0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9df0-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b9df0-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9df0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9df0-108">Prerequisites</span></span>
<span data-ttu-id="b9df0-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9df0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9df0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9df0-111">Permission type</span></span>|<span data-ttu-id="b9df0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9df0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9df0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9df0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9df0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9df0-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b9df0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9df0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9df0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9df0-116">Not supported.</span></span>|
|<span data-ttu-id="b9df0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9df0-117">Application</span></span>|<span data-ttu-id="b9df0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9df0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9df0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9df0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditActivityTypes
```

## <a name="request-headers"></a><span data-ttu-id="b9df0-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9df0-120">Request headers</span></span>
|<span data-ttu-id="b9df0-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9df0-121">Header</span></span>|<span data-ttu-id="b9df0-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b9df0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9df0-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9df0-123">Authorization</span></span>|<span data-ttu-id="b9df0-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9df0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9df0-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9df0-125">Accept</span></span>|<span data-ttu-id="b9df0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9df0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9df0-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9df0-127">Request body</span></span>
<span data-ttu-id="b9df0-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="b9df0-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b9df0-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="b9df0-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b9df0-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9df0-130">Property</span></span>|<span data-ttu-id="b9df0-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9df0-131">Type</span></span>|<span data-ttu-id="b9df0-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9df0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9df0-133">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="b9df0-133">category</span></span>|<span data-ttu-id="b9df0-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9df0-134">String</span></span>|<span data-ttu-id="b9df0-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b9df0-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b9df0-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9df0-136">Response</span></span>
<span data-ttu-id="b9df0-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9df0-137">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9df0-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9df0-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9df0-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9df0-139">Request</span></span>
<span data-ttu-id="b9df0-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9df0-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents/getAuditActivityTypes(category='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b9df0-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9df0-141">Response</span></span>
<span data-ttu-id="b9df0-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9df0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





