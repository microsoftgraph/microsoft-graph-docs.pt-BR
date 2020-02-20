---
title: Obter pfxUserCertificate
description: Leia as propriedades e as relações do objeto pfxUserCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 68064d2998f9915c137de96bcdeab66f8350dc89
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160798"
---
# <a name="get-pfxusercertificate"></a><span data-ttu-id="de13c-103">Obter pfxUserCertificate</span><span class="sxs-lookup"><span data-stu-id="de13c-103">Get pfxUserCertificate</span></span>

> <span data-ttu-id="de13c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="de13c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="de13c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="de13c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="de13c-106">Leia as propriedades e as relações do objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="de13c-106">Read properties and relationships of the [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="de13c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="de13c-107">Prerequisites</span></span>
<span data-ttu-id="de13c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de13c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de13c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de13c-110">Permission type</span></span>|<span data-ttu-id="de13c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="de13c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de13c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de13c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="de13c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="de13c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="de13c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de13c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de13c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="de13c-115">Not supported.</span></span>|
|<span data-ttu-id="de13c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de13c-116">Application</span></span>|<span data-ttu-id="de13c-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="de13c-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de13c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de13c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /pfxUserCertificates/{pfxUserCertificatesId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de13c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="de13c-119">Optional query parameters</span></span>
<span data-ttu-id="de13c-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="de13c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="de13c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de13c-121">Request headers</span></span>
|<span data-ttu-id="de13c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="de13c-122">Header</span></span>|<span data-ttu-id="de13c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="de13c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de13c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="de13c-124">Authorization</span></span>|<span data-ttu-id="de13c-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de13c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de13c-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="de13c-126">Accept</span></span>|<span data-ttu-id="de13c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="de13c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de13c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de13c-128">Request body</span></span>
<span data-ttu-id="de13c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de13c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de13c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="de13c-130">Response</span></span>
<span data-ttu-id="de13c-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de13c-131">If successful, this method returns a `200 OK` response code and [pfxUserCertificate](../resources/intune-raimportcerts-pfxusercertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de13c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="de13c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="de13c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de13c-133">Request</span></span>
<span data-ttu-id="de13c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="de13c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/pfxUserCertificates/{pfxUserCertificatesId}
```

### <a name="response"></a><span data-ttu-id="de13c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="de13c-135">Response</span></span>
<span data-ttu-id="de13c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="de13c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "value": {
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
}
```





