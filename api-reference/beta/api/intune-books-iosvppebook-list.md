---
title: Listar iosVppEBooks
description: Listar propriedades e relações dos objetos iosVppEBook.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: adc0b809b17b02a57fe00ae701d424b0c41b37ef
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133203"
---
# <a name="list-iosvppebooks"></a><span data-ttu-id="3bd70-103">Listar iosVppEBooks</span><span class="sxs-lookup"><span data-stu-id="3bd70-103">List iosVppEBooks</span></span>

<span data-ttu-id="3bd70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bd70-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bd70-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3bd70-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bd70-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bd70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bd70-107">Listar propriedades e relações dos objetos [iosVppEBook](../resources/intune-books-iosvppebook.md).</span><span class="sxs-lookup"><span data-stu-id="3bd70-107">List properties and relationships of the [iosVppEBook](../resources/intune-books-iosvppebook.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bd70-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3bd70-108">Prerequisites</span></span>
<span data-ttu-id="3bd70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bd70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bd70-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bd70-111">Permission type</span></span>|<span data-ttu-id="3bd70-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3bd70-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bd70-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bd70-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bd70-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd70-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3bd70-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bd70-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bd70-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bd70-116">Not supported.</span></span>|
|<span data-ttu-id="3bd70-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3bd70-117">Application</span></span>|<span data-ttu-id="3bd70-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bd70-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bd70-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bd70-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="3bd70-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bd70-120">Request headers</span></span>
|<span data-ttu-id="3bd70-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3bd70-121">Header</span></span>|<span data-ttu-id="3bd70-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3bd70-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bd70-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bd70-123">Authorization</span></span>|<span data-ttu-id="3bd70-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bd70-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bd70-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3bd70-125">Accept</span></span>|<span data-ttu-id="3bd70-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bd70-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bd70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bd70-127">Request body</span></span>
<span data-ttu-id="3bd70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bd70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bd70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bd70-129">Response</span></span>
<span data-ttu-id="3bd70-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosVppEBook](../resources/intune-books-iosvppebook.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bd70-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppEBook](../resources/intune-books-iosvppebook.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bd70-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bd70-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bd70-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bd70-132">Request</span></span>
<span data-ttu-id="3bd70-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bd70-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
```

### <a name="response"></a><span data-ttu-id="3bd70-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bd70-134">Response</span></span>
<span data-ttu-id="3bd70-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bd70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1171

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppEBook",
      "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
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
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
      "appleId": "Apple Id value",
      "vppOrganizationName": "Vpp Organization Name value",
      "genres": [
        "Genres value"
      ],
      "language": "Language value",
      "seller": "Seller value",
      "totalLicenseCount": 1,
      "usedLicenseCount": 0,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




