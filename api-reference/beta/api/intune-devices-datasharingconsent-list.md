---
title: Lista dataSharingConsents
description: Lista as propriedades e os relacionamentos dos objetos dataSharingConsent.
ms.openlocfilehash: 1bc40b927ae03796e5b70c20ce806d78c0f56510
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040499"
---
# <a name="list-datasharingconsents"></a><span data-ttu-id="9ab41-103">Lista dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="9ab41-103">List dataSharingConsents</span></span>

> <span data-ttu-id="9ab41-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9ab41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ab41-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9ab41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ab41-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9ab41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ab41-107">Lista as propriedades e os relacionamentos dos objetos [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="9ab41-107">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9ab41-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ab41-108">Prerequisites</span></span>
<span data-ttu-id="9ab41-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ab41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ab41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ab41-111">Permission type</span></span>|<span data-ttu-id="9ab41-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ab41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ab41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ab41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ab41-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ab41-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9ab41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ab41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ab41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ab41-116">Not supported.</span></span>|
|<span data-ttu-id="9ab41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ab41-117">Application</span></span>|<span data-ttu-id="9ab41-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ab41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ab41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ab41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="9ab41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab41-120">Request headers</span></span>
|<span data-ttu-id="9ab41-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ab41-121">Header</span></span>|<span data-ttu-id="9ab41-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ab41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ab41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ab41-123">Authorization</span></span>|<span data-ttu-id="9ab41-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ab41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ab41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ab41-125">Accept</span></span>|<span data-ttu-id="9ab41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ab41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ab41-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab41-127">Request body</span></span>
<span data-ttu-id="9ab41-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ab41-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ab41-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab41-129">Response</span></span>
<span data-ttu-id="9ab41-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ab41-130">If successful, this method returns a `200 OK` response code and a collection of [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ab41-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ab41-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9ab41-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ab41-132">Request</span></span>
<span data-ttu-id="9ab41-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ab41-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
```

### <a name="response"></a><span data-ttu-id="9ab41-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ab41-134">Response</span></span>
<span data-ttu-id="9ab41-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ab41-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 447

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.dataSharingConsent",
      "id": "333387f7-87f7-3333-f787-3333f7873333",
      "serviceDisplayName": "Service Display Name value",
      "termsUrl": "https://example.com/termsUrl/",
      "granted": true,
      "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
      "grantedByUpn": "Granted By Upn value",
      "grantedByUserId": "Granted By User Id value"
    }
  ]
}
```





