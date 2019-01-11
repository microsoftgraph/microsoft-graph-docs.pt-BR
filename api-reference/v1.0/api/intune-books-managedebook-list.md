---
title: Listar managedEBooks
description: Lista propriedades e relações dos objetos managedEBook.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: baf4b7275d9c6709a2d8959d2f82b806d0df01f4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807067"
---
# <a name="list-managedebooks"></a><span data-ttu-id="334ae-103">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="334ae-103">List managedEBooks</span></span>

> <span data-ttu-id="334ae-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="334ae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="334ae-105">Listar propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="334ae-105">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="334ae-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="334ae-106">Prerequisites</span></span>
<span data-ttu-id="334ae-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="334ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="334ae-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="334ae-109">Permission type</span></span>|<span data-ttu-id="334ae-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="334ae-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="334ae-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="334ae-111">Delegated (work or school account)</span></span>|<span data-ttu-id="334ae-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="334ae-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="334ae-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="334ae-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="334ae-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="334ae-114">Not supported.</span></span>|
|<span data-ttu-id="334ae-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="334ae-115">Application</span></span>|<span data-ttu-id="334ae-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="334ae-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="334ae-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="334ae-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="334ae-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="334ae-118">Request headers</span></span>
|<span data-ttu-id="334ae-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="334ae-119">Header</span></span>|<span data-ttu-id="334ae-120">Valor</span><span class="sxs-lookup"><span data-stu-id="334ae-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="334ae-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="334ae-121">Authorization</span></span>|<span data-ttu-id="334ae-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="334ae-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="334ae-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="334ae-123">Accept</span></span>|<span data-ttu-id="334ae-124">application/json</span><span class="sxs-lookup"><span data-stu-id="334ae-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="334ae-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="334ae-125">Request body</span></span>
<span data-ttu-id="334ae-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="334ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="334ae-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="334ae-127">Response</span></span>
<span data-ttu-id="334ae-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedEBook](../resources/intune-books-managedebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="334ae-128">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="334ae-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="334ae-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="334ae-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="334ae-130">Request</span></span>
<span data-ttu-id="334ae-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="334ae-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="334ae-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="334ae-132">Response</span></span>
<span data-ttu-id="334ae-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="334ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBook",
      "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
      "largeCover": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "informationUrl": "https://example.com/informationUrl/",
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
    }
  ]
}
```



