---
title: Listar pfxUserCertificates
description: Listar propriedades e relações dos objetos pfxUserCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 748aa490788729b921a89aacb03caf21d1e2115f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868275"
---
# <a name="list-pfxusercertificates"></a><span data-ttu-id="07f81-103">Listar pfxUserCertificates</span><span class="sxs-lookup"><span data-stu-id="07f81-103">List pfxUserCertificates</span></span>

<span data-ttu-id="07f81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07f81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07f81-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07f81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07f81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07f81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07f81-107">Listar propriedades e relações dos objetos [pfxUserCertificate.](../resources/intune-raimportcerts-pfxusercertificate.md)</span><span class="sxs-lookup"><span data-stu-id="07f81-107">List properties and relationships of the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07f81-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07f81-108">Prerequisites</span></span>
<span data-ttu-id="07f81-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07f81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07f81-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07f81-111">Permission type</span></span>|<span data-ttu-id="07f81-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07f81-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07f81-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07f81-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07f81-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07f81-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="07f81-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07f81-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07f81-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07f81-116">Not supported.</span></span>|
|<span data-ttu-id="07f81-117">Application</span><span class="sxs-lookup"><span data-stu-id="07f81-117">Application</span></span>|<span data-ttu-id="07f81-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07f81-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07f81-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07f81-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxUserCertificates
```

## <a name="request-headers"></a><span data-ttu-id="07f81-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07f81-120">Request headers</span></span>
|<span data-ttu-id="07f81-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07f81-121">Header</span></span>|<span data-ttu-id="07f81-122">Valor</span><span class="sxs-lookup"><span data-stu-id="07f81-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07f81-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="07f81-123">Authorization</span></span>|<span data-ttu-id="07f81-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07f81-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07f81-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07f81-125">Accept</span></span>|<span data-ttu-id="07f81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07f81-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07f81-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07f81-127">Request body</span></span>
<span data-ttu-id="07f81-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="07f81-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07f81-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="07f81-129">Response</span></span>
<span data-ttu-id="07f81-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07f81-130">If successful, this method returns a `200 OK` response code and a collection of [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07f81-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07f81-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="07f81-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07f81-132">Request</span></span>
<span data-ttu-id="07f81-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07f81-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxUserCertificates
```

### <a name="response"></a><span data-ttu-id="07f81-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="07f81-134">Response</span></span>
<span data-ttu-id="07f81-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07f81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




