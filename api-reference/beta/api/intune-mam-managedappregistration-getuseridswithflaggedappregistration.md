---
title: função getUserIdsWithFlaggedAppRegistration
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 7f57ab3af48ac7e815b914be3339435d6be58fc4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329376"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="e8e52-103">função getUserIdsWithFlaggedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e8e52-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="e8e52-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8e52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8e52-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8e52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8e52-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e8e52-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8e52-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8e52-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8e52-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8e52-108">Prerequisites</span></span>
<span data-ttu-id="e8e52-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8e52-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8e52-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8e52-111">Permission type</span></span>|<span data-ttu-id="e8e52-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8e52-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8e52-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8e52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8e52-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8e52-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e8e52-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8e52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8e52-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8e52-116">Not supported.</span></span>|
|<span data-ttu-id="e8e52-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8e52-117">Application</span></span>|<span data-ttu-id="e8e52-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8e52-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8e52-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8e52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="e8e52-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e52-120">Request headers</span></span>
|<span data-ttu-id="e8e52-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8e52-121">Header</span></span>|<span data-ttu-id="e8e52-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e8e52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8e52-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8e52-123">Authorization</span></span>|<span data-ttu-id="e8e52-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8e52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8e52-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8e52-125">Accept</span></span>|<span data-ttu-id="e8e52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8e52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8e52-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e52-127">Request body</span></span>
<span data-ttu-id="e8e52-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8e52-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8e52-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8e52-129">Response</span></span>
<span data-ttu-id="e8e52-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma Coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8e52-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8e52-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8e52-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8e52-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8e52-132">Request</span></span>
<span data-ttu-id="e8e52-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8e52-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="e8e52-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8e52-134">Response</span></span>
<span data-ttu-id="e8e52-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8e52-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```





