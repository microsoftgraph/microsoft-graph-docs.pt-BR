---
title: Obter userPFXCertificate
description: Leia as propriedades e os relacionamentos do objeto userPFXCertificate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 464c3e5b9cbbc87987c31d4717028b75ba25dc85
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404978"
---
# <a name="get-userpfxcertificate"></a><span data-ttu-id="87e7c-103">Obter userPFXCertificate</span><span class="sxs-lookup"><span data-stu-id="87e7c-103">Get userPFXCertificate</span></span>

> <span data-ttu-id="87e7c-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="87e7c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="87e7c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87e7c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87e7c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="87e7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87e7c-107">Leia as propriedades e os relacionamentos do objeto [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="87e7c-107">Read properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87e7c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87e7c-108">Prerequisites</span></span>
<span data-ttu-id="87e7c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="87e7c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="87e7c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87e7c-111">Permission type</span></span>|<span data-ttu-id="87e7c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87e7c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87e7c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87e7c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87e7c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87e7c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87e7c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87e7c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87e7c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87e7c-116">Not supported.</span></span>|
|<span data-ttu-id="87e7c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87e7c-117">Application</span></span>|<span data-ttu-id="87e7c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87e7c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87e7c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87e7c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87e7c-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="87e7c-120">Optional query parameters</span></span>
<span data-ttu-id="87e7c-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="87e7c-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="87e7c-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87e7c-122">Request headers</span></span>
|<span data-ttu-id="87e7c-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87e7c-123">Header</span></span>|<span data-ttu-id="87e7c-124">Valor</span><span class="sxs-lookup"><span data-stu-id="87e7c-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87e7c-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="87e7c-125">Authorization</span></span>|<span data-ttu-id="87e7c-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87e7c-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87e7c-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87e7c-127">Accept</span></span>|<span data-ttu-id="87e7c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="87e7c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87e7c-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87e7c-129">Request body</span></span>
<span data-ttu-id="87e7c-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="87e7c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87e7c-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="87e7c-131">Response</span></span>
<span data-ttu-id="87e7c-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87e7c-132">If successful, this method returns a `200 OK` response code and [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87e7c-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87e7c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="87e7c-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87e7c-134">Request</span></span>
<span data-ttu-id="87e7c-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87e7c-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates/{userPFXCertificateId}
```

### <a name="response"></a><span data-ttu-id="87e7c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="87e7c-136">Response</span></span>
<span data-ttu-id="87e7c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87e7c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




