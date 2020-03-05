---
title: Listar pfxUserCertificates
description: Listar Propriedades e relações dos objetos pfxUserCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e3b16b9328b4cae2d795e3d623a7844060a45de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42460035"
---
# <a name="list-pfxusercertificates"></a><span data-ttu-id="b6f8f-103">Listar pfxUserCertificates</span><span class="sxs-lookup"><span data-stu-id="b6f8f-103">List pfxUserCertificates</span></span>

<span data-ttu-id="b6f8f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b6f8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6f8f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6f8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6f8f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6f8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6f8f-107">Listar Propriedades e relações dos objetos [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="b6f8f-107">List properties and relationships of the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6f8f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6f8f-108">Prerequisites</span></span>
<span data-ttu-id="b6f8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6f8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6f8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6f8f-111">Permission type</span></span>|<span data-ttu-id="b6f8f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6f8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6f8f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6f8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6f8f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6f8f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b6f8f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6f8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6f8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6f8f-116">Not supported.</span></span>|
|<span data-ttu-id="b6f8f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6f8f-117">Application</span></span>|<span data-ttu-id="b6f8f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6f8f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6f8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6f8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="b6f8f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f8f-120">Request headers</span></span>
|<span data-ttu-id="b6f8f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6f8f-121">Header</span></span>|<span data-ttu-id="b6f8f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6f8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6f8f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6f8f-123">Authorization</span></span>|<span data-ttu-id="b6f8f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6f8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6f8f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6f8f-125">Accept</span></span>|<span data-ttu-id="b6f8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6f8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6f8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f8f-127">Request body</span></span>
<span data-ttu-id="b6f8f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6f8f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6f8f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f8f-129">Response</span></span>
<span data-ttu-id="b6f8f-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6f8f-130">If successful, this method returns a `200 OK` response code and a collection of [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6f8f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6f8f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6f8f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6f8f-132">Request</span></span>
<span data-ttu-id="b6f8f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6f8f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxUserCertificates
```

### <a name="response"></a><span data-ttu-id="b6f8f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6f8f-134">Response</span></span>
<span data-ttu-id="b6f8f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6f8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 894

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.pfxUserCertificate",
      "tenantId": "f9882bcd-2bcd-f988-cd2b-88f9cd2b88f9",
      "userId": "a991071c-071c-a991-1c07-91a91c0791a9",
      "thumbprint": "Thumbprint value",
      "userUpn": "User Upn value",
      "encryptedPfxBlob": "Encrypted Pfx Blob value",
      "encryptedPfxPassword": "Encrypted Pfx Password value",
      "certStartDate": "2017-01-01T00:01:48.7697664-08:00",
      "certExpirationDate": "2016-12-31T23:56:39.3841403-08:00",
      "providerName": "Provider Name value",
      "encryptionKeyName": "Encryption Key Name value",
      "paddingScheme": 13,
      "status": 6,
      "intendedPurpose": 15,
      "createdTime": "2017-01-01T00:03:18.9597073-08:00",
      "isDeleted": true,
      "lastModifiedTime": "2017-01-01T00:03:18.5958204-08:00",
      "eTag": "ETag value"
    }
  ]
}
```





