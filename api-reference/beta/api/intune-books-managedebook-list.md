---
title: Listar managedEBooks
description: Listar propriedades e relações dos objetos managedEBook.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a772a7f8fcb3f273cf0934a60528775dfd5a6e9b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483303"
---
# <a name="list-managedebooks"></a><span data-ttu-id="30e53-103">Listar managedEBooks</span><span class="sxs-lookup"><span data-stu-id="30e53-103">List managedEBooks</span></span>

> <span data-ttu-id="30e53-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="30e53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30e53-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="30e53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30e53-106">Listar propriedades e relações dos objetos [managedEBook](../resources/intune-books-managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="30e53-106">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30e53-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="30e53-107">Prerequisites</span></span>
<span data-ttu-id="30e53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30e53-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30e53-110">Permission type</span></span>|<span data-ttu-id="30e53-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="30e53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30e53-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30e53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30e53-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="30e53-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="30e53-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30e53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30e53-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30e53-115">Not supported.</span></span>|
|<span data-ttu-id="30e53-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30e53-116">Application</span></span>|<span data-ttu-id="30e53-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30e53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30e53-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30e53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="30e53-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="30e53-119">Request headers</span></span>
|<span data-ttu-id="30e53-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="30e53-120">Header</span></span>|<span data-ttu-id="30e53-121">Valor</span><span class="sxs-lookup"><span data-stu-id="30e53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30e53-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="30e53-122">Authorization</span></span>|<span data-ttu-id="30e53-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="30e53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30e53-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="30e53-124">Accept</span></span>|<span data-ttu-id="30e53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30e53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30e53-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30e53-126">Request body</span></span>
<span data-ttu-id="30e53-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="30e53-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30e53-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="30e53-128">Response</span></span>
<span data-ttu-id="30e53-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedEBook](../resources/intune-books-managedebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="30e53-129">If successful, this method returns a `200 OK` response code and a collection of [managedEBook](../resources/intune-books-managedebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30e53-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="30e53-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="30e53-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="30e53-131">Request</span></span>
<span data-ttu-id="30e53-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="30e53-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="30e53-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="30e53-133">Response</span></span>
<span data-ttu-id="30e53-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="30e53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





