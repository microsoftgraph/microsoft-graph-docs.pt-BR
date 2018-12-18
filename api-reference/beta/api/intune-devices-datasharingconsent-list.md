---
title: Lista dataSharingConsents
description: Lista as propriedades e os relacionamentos dos objetos dataSharingConsent.
author: tfitzmac
ms.openlocfilehash: a8d3fd49b8749dc982b70601ae5fbff836d1052c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312618"
---
# <a name="list-datasharingconsents"></a><span data-ttu-id="10e40-103">Lista dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="10e40-103">List dataSharingConsents</span></span>

> <span data-ttu-id="10e40-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="10e40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10e40-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="10e40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10e40-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="10e40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10e40-107">Lista as propriedades e os relacionamentos dos objetos [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .</span><span class="sxs-lookup"><span data-stu-id="10e40-107">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10e40-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10e40-108">Prerequisites</span></span>
<span data-ttu-id="10e40-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10e40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10e40-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10e40-111">Permission type</span></span>|<span data-ttu-id="10e40-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10e40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10e40-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10e40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10e40-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10e40-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="10e40-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10e40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10e40-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10e40-116">Not supported.</span></span>|
|<span data-ttu-id="10e40-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10e40-117">Application</span></span>|<span data-ttu-id="10e40-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10e40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10e40-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10e40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="10e40-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10e40-120">Request headers</span></span>
|<span data-ttu-id="10e40-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10e40-121">Header</span></span>|<span data-ttu-id="10e40-122">Valor</span><span class="sxs-lookup"><span data-stu-id="10e40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10e40-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="10e40-123">Authorization</span></span>|<span data-ttu-id="10e40-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10e40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10e40-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10e40-125">Accept</span></span>|<span data-ttu-id="10e40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10e40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10e40-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10e40-127">Request body</span></span>
<span data-ttu-id="10e40-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="10e40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10e40-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="10e40-129">Response</span></span>
<span data-ttu-id="10e40-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10e40-130">If successful, this method returns a `200 OK` response code and a collection of [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10e40-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10e40-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="10e40-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10e40-132">Request</span></span>
<span data-ttu-id="10e40-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10e40-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
```

### <a name="response"></a><span data-ttu-id="10e40-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="10e40-134">Response</span></span>
<span data-ttu-id="10e40-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10e40-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





