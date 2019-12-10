---
title: Listar enterpriseCodeSigningCertificates
description: Listar Propriedades e relações dos objetos enterpriseCodeSigningCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45587cf1a9cb2985ce0dd560e2f17a8007c329b9
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39921589"
---
# <a name="list-enterprisecodesigningcertificates"></a><span data-ttu-id="bed64-103">Listar enterpriseCodeSigningCertificates</span><span class="sxs-lookup"><span data-stu-id="bed64-103">List enterpriseCodeSigningCertificates</span></span>

> <span data-ttu-id="bed64-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bed64-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bed64-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bed64-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bed64-106">Listar Propriedades e relações dos objetos [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="bed64-106">List properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bed64-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bed64-107">Prerequisites</span></span>
<span data-ttu-id="bed64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bed64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bed64-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bed64-110">Permission type</span></span>|<span data-ttu-id="bed64-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="bed64-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bed64-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bed64-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bed64-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bed64-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bed64-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bed64-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bed64-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bed64-115">Not supported.</span></span>|
|<span data-ttu-id="bed64-116">Application</span><span class="sxs-lookup"><span data-stu-id="bed64-116">Application</span></span>|<span data-ttu-id="bed64-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bed64-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bed64-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bed64-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates
```

## <a name="request-headers"></a><span data-ttu-id="bed64-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bed64-119">Request headers</span></span>
|<span data-ttu-id="bed64-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="bed64-120">Header</span></span>|<span data-ttu-id="bed64-121">Valor</span><span class="sxs-lookup"><span data-stu-id="bed64-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bed64-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="bed64-122">Authorization</span></span>|<span data-ttu-id="bed64-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bed64-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bed64-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="bed64-124">Accept</span></span>|<span data-ttu-id="bed64-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bed64-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bed64-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bed64-126">Request body</span></span>
<span data-ttu-id="bed64-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="bed64-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bed64-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="bed64-128">Response</span></span>
<span data-ttu-id="bed64-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bed64-129">If successful, this method returns a `200 OK` response code and a collection of [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bed64-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bed64-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bed64-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bed64-131">Request</span></span>
<span data-ttu-id="bed64-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bed64-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates
```

### <a name="response"></a><span data-ttu-id="bed64-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="bed64-133">Response</span></span>
<span data-ttu-id="bed64-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bed64-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
      "id": "b20d3703-3703-b20d-0337-0db203370db2",
      "content": "Y29udGVudA==",
      "status": "provisioned",
      "subjectName": "Subject Name value",
      "subject": "Subject value",
      "issuerName": "Issuer Name value",
      "issuer": "Issuer value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
    }
  ]
}
```





