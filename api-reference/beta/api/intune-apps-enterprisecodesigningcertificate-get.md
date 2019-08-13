---
title: Obter enterpriseCodeSigningCertificate
description: Leia as propriedades e as relações do objeto enterpriseCodeSigningCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9032028014468b7e871da2ae6d8c3f780cc10267
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330955"
---
# <a name="get-enterprisecodesigningcertificate"></a><span data-ttu-id="d1cab-103">Obter enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="d1cab-103">Get enterpriseCodeSigningCertificate</span></span>

> <span data-ttu-id="d1cab-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d1cab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1cab-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d1cab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1cab-106">Leia as propriedades e as relações do objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="d1cab-106">Read properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d1cab-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d1cab-107">Prerequisites</span></span>
<span data-ttu-id="d1cab-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1cab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1cab-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d1cab-110">Permission type</span></span>|<span data-ttu-id="d1cab-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d1cab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d1cab-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d1cab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d1cab-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1cab-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d1cab-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d1cab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d1cab-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d1cab-115">Not supported.</span></span>|
|<span data-ttu-id="d1cab-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d1cab-116">Application</span></span>|<span data-ttu-id="d1cab-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d1cab-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d1cab-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d1cab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d1cab-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d1cab-119">Optional query parameters</span></span>
<span data-ttu-id="d1cab-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d1cab-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1cab-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d1cab-121">Request headers</span></span>
|<span data-ttu-id="d1cab-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d1cab-122">Header</span></span>|<span data-ttu-id="d1cab-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d1cab-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d1cab-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d1cab-124">Authorization</span></span>|<span data-ttu-id="d1cab-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1cab-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d1cab-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d1cab-126">Accept</span></span>|<span data-ttu-id="d1cab-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d1cab-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d1cab-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d1cab-128">Request body</span></span>
<span data-ttu-id="d1cab-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d1cab-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1cab-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1cab-130">Response</span></span>
<span data-ttu-id="d1cab-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d1cab-131">If successful, this method returns a `200 OK` response code and [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d1cab-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d1cab-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d1cab-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d1cab-133">Request</span></span>
<span data-ttu-id="d1cab-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d1cab-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

### <a name="response"></a><span data-ttu-id="d1cab-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d1cab-135">Response</span></span>
<span data-ttu-id="d1cab-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d1cab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 478

{
  "value": {
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
}
```






