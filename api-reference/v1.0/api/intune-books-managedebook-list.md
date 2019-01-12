---
title: Listar managedEBooks
description: Lista propriedades e relações dos objetos managedEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7b9801e76f475f42f8e7f538e710d00aea63c2e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981704"
---
# <a name="list-managedebooks"></a><span data-ttu-id="0b41d-103">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="0b41d-103">List managedEBooks</span></span>

> <span data-ttu-id="0b41d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0b41d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b41d-105">Listar propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="0b41d-105">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b41d-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0b41d-106">Prerequisites</span></span>
<span data-ttu-id="0b41d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b41d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b41d-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b41d-109">Permission type</span></span>|<span data-ttu-id="0b41d-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0b41d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b41d-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b41d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b41d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b41d-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0b41d-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b41d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b41d-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b41d-114">Not supported.</span></span>|
|<span data-ttu-id="0b41d-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b41d-115">Application</span></span>|<span data-ttu-id="0b41d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b41d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b41d-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b41d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="0b41d-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b41d-118">Request headers</span></span>
|<span data-ttu-id="0b41d-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0b41d-119">Header</span></span>|<span data-ttu-id="0b41d-120">Valor</span><span class="sxs-lookup"><span data-stu-id="0b41d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b41d-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b41d-121">Authorization</span></span>|<span data-ttu-id="0b41d-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b41d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b41d-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0b41d-123">Accept</span></span>|<span data-ttu-id="0b41d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0b41d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b41d-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b41d-125">Request body</span></span>
<span data-ttu-id="0b41d-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b41d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b41d-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b41d-127">Response</span></span>
<span data-ttu-id="0b41d-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedEBook](../resources/intune-books-managedebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b41d-128">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b41d-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0b41d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b41d-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b41d-130">Request</span></span>
<span data-ttu-id="0b41d-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b41d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="0b41d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b41d-132">Response</span></span>
<span data-ttu-id="0b41d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b41d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



