---
title: Listar mobileAppContents
description: Listar propriedades e relações dos objetos mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7fc06ee7a702eed2f1226335acb94ccf7edc3a18
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829810"
---
# <a name="list-mobileappcontents"></a><span data-ttu-id="50330-103">Listar mobileAppContents</span><span class="sxs-lookup"><span data-stu-id="50330-103">List mobileAppContents</span></span>

> <span data-ttu-id="50330-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="50330-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="50330-105">Listar propriedades e relações dos objetos [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span><span class="sxs-lookup"><span data-stu-id="50330-105">List properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50330-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50330-106">Prerequisites</span></span>
<span data-ttu-id="50330-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50330-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50330-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50330-109">Permission type</span></span>|<span data-ttu-id="50330-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50330-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50330-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50330-111">Delegated (work or school account)</span></span>|<span data-ttu-id="50330-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="50330-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="50330-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50330-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50330-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50330-114">Not supported.</span></span>|
|<span data-ttu-id="50330-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50330-115">Application</span></span>|<span data-ttu-id="50330-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50330-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50330-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50330-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="50330-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50330-118">Request headers</span></span>
|<span data-ttu-id="50330-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50330-119">Header</span></span>|<span data-ttu-id="50330-120">Valor</span><span class="sxs-lookup"><span data-stu-id="50330-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50330-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="50330-121">Authorization</span></span>|<span data-ttu-id="50330-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50330-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50330-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50330-123">Accept</span></span>|<span data-ttu-id="50330-124">application/json</span><span class="sxs-lookup"><span data-stu-id="50330-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50330-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50330-125">Request body</span></span>
<span data-ttu-id="50330-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50330-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50330-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="50330-127">Response</span></span>
<span data-ttu-id="50330-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [mobileAppContent](../resources/intune-apps-mobileappcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50330-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppContent](../resources/intune-apps-mobileappcontent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50330-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50330-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="50330-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50330-130">Request</span></span>
<span data-ttu-id="50330-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50330-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
```

### <a name="response"></a><span data-ttu-id="50330-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="50330-132">Response</span></span>
<span data-ttu-id="50330-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50330-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 148

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContent",
      "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
    }
  ]
}
```



