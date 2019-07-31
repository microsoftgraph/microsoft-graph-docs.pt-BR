---
title: Listar userPFXCertificates
description: Listar Propriedades e relações dos objetos userPFXCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cb11f19a3c89fbe1c643db4c0861a7a6d797213d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984213"
---
# <a name="list-userpfxcertificates"></a><span data-ttu-id="46e07-103">Listar userPFXCertificates</span><span class="sxs-lookup"><span data-stu-id="46e07-103">List userPFXCertificates</span></span>

> <span data-ttu-id="46e07-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="46e07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46e07-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46e07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46e07-106">Listar Propriedades e relações dos objetos [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="46e07-106">List properties and relationships of the [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46e07-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="46e07-107">Prerequisites</span></span>
<span data-ttu-id="46e07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46e07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46e07-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46e07-110">Permission type</span></span>|<span data-ttu-id="46e07-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="46e07-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46e07-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46e07-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46e07-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="46e07-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="46e07-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46e07-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46e07-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46e07-115">Not supported.</span></span>|
|<span data-ttu-id="46e07-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46e07-116">Application</span></span>|<span data-ttu-id="46e07-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46e07-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46e07-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46e07-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userPfxCertificates
```

## <a name="request-headers"></a><span data-ttu-id="46e07-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46e07-119">Request headers</span></span>
|<span data-ttu-id="46e07-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="46e07-120">Header</span></span>|<span data-ttu-id="46e07-121">Valor</span><span class="sxs-lookup"><span data-stu-id="46e07-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46e07-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="46e07-122">Authorization</span></span>|<span data-ttu-id="46e07-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46e07-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46e07-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="46e07-124">Accept</span></span>|<span data-ttu-id="46e07-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46e07-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46e07-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46e07-126">Request body</span></span>
<span data-ttu-id="46e07-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46e07-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46e07-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="46e07-128">Response</span></span>
<span data-ttu-id="46e07-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46e07-129">If successful, this method returns a `200 OK` response code and a collection of [userPFXCertificate](../resources/intune-raimportcerts-userpfxcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46e07-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="46e07-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="46e07-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46e07-131">Request</span></span>
<span data-ttu-id="46e07-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="46e07-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userPfxCertificates
```

### <a name="response"></a><span data-ttu-id="46e07-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="46e07-133">Response</span></span>
<span data-ttu-id="46e07-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46e07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





