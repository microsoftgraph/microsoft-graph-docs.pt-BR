---
title: Acessar managedEBook
description: Propriedades de leitura e relações do objeto managedEBook.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9dcb8524faa39a36d61748f61fe245c688578445
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870984"
---
# <a name="get-managedebook"></a><span data-ttu-id="4d1ca-103">Acessar managedEBook</span><span class="sxs-lookup"><span data-stu-id="4d1ca-103">Get managedEBook</span></span>

> <span data-ttu-id="4d1ca-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4d1ca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4d1ca-105">Leia as propriedades e as relações do objeto [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="4d1ca-105">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4d1ca-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4d1ca-106">Prerequisites</span></span>
<span data-ttu-id="4d1ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d1ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d1ca-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d1ca-109">Permission type</span></span>|<span data-ttu-id="4d1ca-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4d1ca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4d1ca-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d1ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4d1ca-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d1ca-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4d1ca-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d1ca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4d1ca-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d1ca-114">Not supported.</span></span>|
|<span data-ttu-id="4d1ca-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d1ca-115">Application</span></span>|<span data-ttu-id="4d1ca-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d1ca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4d1ca-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d1ca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4d1ca-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4d1ca-118">Optional query parameters</span></span>
<span data-ttu-id="4d1ca-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4d1ca-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4d1ca-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d1ca-120">Request headers</span></span>
|<span data-ttu-id="4d1ca-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4d1ca-121">Header</span></span>|<span data-ttu-id="4d1ca-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4d1ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4d1ca-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d1ca-123">Authorization</span></span>|<span data-ttu-id="4d1ca-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d1ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4d1ca-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4d1ca-125">Accept</span></span>|<span data-ttu-id="4d1ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4d1ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d1ca-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d1ca-127">Request body</span></span>
<span data-ttu-id="4d1ca-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d1ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d1ca-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d1ca-129">Response</span></span>
<span data-ttu-id="4d1ca-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [managedEBook](../resources/intune-books-managedebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d1ca-130">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune-books-managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d1ca-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d1ca-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="4d1ca-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d1ca-132">Request</span></span>
<span data-ttu-id="4d1ca-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4d1ca-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="4d1ca-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d1ca-134">Response</span></span>
<span data-ttu-id="4d1ca-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4d1ca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
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
}
```



