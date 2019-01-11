---
title: Listar managedApps
description: Listar propriedades e relações dos objetos managedApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0981060d750fcd7593516a7ef1cd366de5f9de2e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869808"
---
# <a name="list-managedapps"></a><span data-ttu-id="51eca-103">Listar managedApps</span><span class="sxs-lookup"><span data-stu-id="51eca-103">List managedApps</span></span>

> <span data-ttu-id="51eca-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="51eca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51eca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="51eca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51eca-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="51eca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51eca-107">Listar propriedades e relações dos objetos [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="51eca-107">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="51eca-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51eca-108">Prerequisites</span></span>
<span data-ttu-id="51eca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51eca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51eca-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51eca-111">Permission type</span></span>|<span data-ttu-id="51eca-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="51eca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51eca-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51eca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51eca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="51eca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="51eca-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51eca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51eca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51eca-116">Not supported.</span></span>|
|<span data-ttu-id="51eca-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51eca-117">Application</span></span>|<span data-ttu-id="51eca-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51eca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51eca-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51eca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="51eca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51eca-120">Request headers</span></span>
|<span data-ttu-id="51eca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51eca-121">Header</span></span>|<span data-ttu-id="51eca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51eca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51eca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51eca-123">Authorization</span></span>|<span data-ttu-id="51eca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51eca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51eca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51eca-125">Accept</span></span>|<span data-ttu-id="51eca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51eca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51eca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51eca-127">Request body</span></span>
<span data-ttu-id="51eca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="51eca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51eca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="51eca-129">Response</span></span>
<span data-ttu-id="51eca-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedApp](../resources/intune-apps-managedapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51eca-130">If successful, this method returns a `200 OK` response code and a collection of [managedApp](../resources/intune-apps-managedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51eca-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51eca-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="51eca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51eca-132">Request</span></span>
<span data-ttu-id="51eca-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51eca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="51eca-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="51eca-134">Response</span></span>
<span data-ttu-id="51eca-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51eca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 961

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedApp",
      "id": "f687dd85-dd85-f687-85dd-87f685dd87f6",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "uploadState": 11,
      "publishingState": "processing",
      "appAvailability": "lineOfBusiness",
      "version": "Version value"
    }
  ]
}
```





