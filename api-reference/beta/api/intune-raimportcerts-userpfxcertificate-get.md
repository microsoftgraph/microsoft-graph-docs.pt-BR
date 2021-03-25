---
title: Obter userPFXCertificate
description: Leia propriedades e relações do objeto userPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 71af940118bc256f9212ab9e19442802f672d1a2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152233"
---
# <a name="get-userpfxcertificate"></a><span data-ttu-id="74efb-103">Obter userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="74efb-103">Get userPFXCertificate</span></span>

<span data-ttu-id="74efb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74efb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74efb-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="74efb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74efb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="74efb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74efb-107">Leia propriedades e relações do [objeto userPFXCertificate.](../resources/intune-raimportcerts-userpfxcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="74efb-107">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74efb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="74efb-108">Prerequisites</span></span>
<span data-ttu-id="74efb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="74efb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74efb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="74efb-111">Permission type</span></span>|<span data-ttu-id="74efb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="74efb-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74efb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="74efb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74efb-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74efb-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74efb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="74efb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74efb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="74efb-116">Not supported.</span></span>|
|<span data-ttu-id="74efb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="74efb-117">Application</span></span>|<span data-ttu-id="74efb-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74efb-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="74efb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="74efb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="74efb-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="74efb-120">Optional query parameters</span></span>
<span data-ttu-id="74efb-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="74efb-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="74efb-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="74efb-122">Request headers</span></span>
|<span data-ttu-id="74efb-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="74efb-123">Header</span></span>|<span data-ttu-id="74efb-124">Valor</span><span class="sxs-lookup"><span data-stu-id="74efb-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74efb-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="74efb-125">Authorization</span></span>|<span data-ttu-id="74efb-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="74efb-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74efb-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="74efb-127">Accept</span></span>|<span data-ttu-id="74efb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="74efb-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74efb-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="74efb-129">Request body</span></span>
<span data-ttu-id="74efb-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="74efb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="74efb-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="74efb-131">Response</span></span>
<span data-ttu-id="74efb-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="74efb-132">If successful, this method returns a `200 OK` response code and [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74efb-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="74efb-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="74efb-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="74efb-134">Request</span></span>
<span data-ttu-id="74efb-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="74efb-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

### <a name="response"></a><span data-ttu-id="74efb-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="74efb-136">Response</span></span>
<span data-ttu-id="74efb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="74efb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 742

{
  "value": {
    "@odata.type": "#microsoft.graph.userPFXCertificate",
    "id": "045c159b-159b-045c-9b15-5c049b155c04",
    "thumbprint": "Thumbprint value",
    "intendedPurpose": "smimeEncryption",
    "userPrincipalName": "User Principal Name value",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "providerName": "Provider Name value",
    "keyName": "Key Name value",
    "paddingScheme": "pkcs1",
    "encryptedPfxBlob": "ZW5jcnlwdGVkUGZ4QmxvYg==",
    "encryptedPfxPassword": "Encrypted Pfx Password value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




