---
title: Listar userPFXCertificates
description: Listar Propriedades e relações dos objetos userPFXCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 07c502793fedf6d3b96dc2040d6ea6ec5b630384
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731145"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="6def4-103">Listar userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="6def4-103">List userPFXCertificates</span></span>

<span data-ttu-id="6def4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6def4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6def4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6def4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6def4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6def4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6def4-107">Listar Propriedades e relações dos objetos [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="6def4-107">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6def4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6def4-108">Prerequisites</span></span>
<span data-ttu-id="6def4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6def4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6def4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6def4-111">Permission type</span></span>|<span data-ttu-id="6def4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6def4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6def4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6def4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6def4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6def4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6def4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6def4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6def4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6def4-116">Not supported.</span></span>|
|<span data-ttu-id="6def4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6def4-117">Application</span></span>|<span data-ttu-id="6def4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6def4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6def4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6def4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="6def4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6def4-120">Request headers</span></span>
|<span data-ttu-id="6def4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6def4-121">Header</span></span>|<span data-ttu-id="6def4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6def4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6def4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6def4-123">Authorization</span></span>|<span data-ttu-id="6def4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6def4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6def4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6def4-125">Accept</span></span>|<span data-ttu-id="6def4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6def4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6def4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6def4-127">Request body</span></span>
<span data-ttu-id="6def4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6def4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6def4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6def4-129">Response</span></span>
<span data-ttu-id="6def4-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6def4-130">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6def4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6def4-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6def4-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6def4-132">Request</span></span>
<span data-ttu-id="6def4-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6def4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="6def4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6def4-134">Response</span></span>
<span data-ttu-id="6def4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6def4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 784

{
  "value": [
    {
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
  ]
}
```





