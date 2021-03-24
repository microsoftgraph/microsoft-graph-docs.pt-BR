---
title: Obter enterpriseCodeSigningCertificate
description: Ler propriedades e relações do objeto enterpriseCodeSigningCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fdca484fca877cdad05e5d4b5acf2a3ef3eed02e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144302"
---
# <a name="get-enterprisecodesigningcertificate"></a><span data-ttu-id="c857e-103">Obter enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="c857e-103">Get enterpriseCodeSigningCertificate</span></span>

<span data-ttu-id="c857e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c857e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c857e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c857e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c857e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c857e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c857e-107">Ler propriedades e relações do [objeto enterpriseCodeSigningCertificate.](../resources/intune-apps-enterprisecodesigningcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="c857e-107">Read properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c857e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c857e-108">Prerequisites</span></span>
<span data-ttu-id="c857e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c857e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c857e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c857e-111">Permission type</span></span>|<span data-ttu-id="c857e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c857e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c857e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c857e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c857e-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c857e-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c857e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c857e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c857e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c857e-116">Not supported.</span></span>|
|<span data-ttu-id="c857e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c857e-117">Application</span></span>|<span data-ttu-id="c857e-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c857e-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c857e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c857e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c857e-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c857e-120">Optional query parameters</span></span>
<span data-ttu-id="c857e-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c857e-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c857e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c857e-122">Request headers</span></span>
|<span data-ttu-id="c857e-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c857e-123">Header</span></span>|<span data-ttu-id="c857e-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c857e-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c857e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c857e-125">Authorization</span></span>|<span data-ttu-id="c857e-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c857e-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c857e-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c857e-127">Accept</span></span>|<span data-ttu-id="c857e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c857e-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c857e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c857e-129">Request body</span></span>
<span data-ttu-id="c857e-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c857e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c857e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c857e-131">Response</span></span>
<span data-ttu-id="c857e-132">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c857e-132">If successful, this method returns a `200 OK` response code and [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c857e-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c857e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c857e-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c857e-134">Request</span></span>
<span data-ttu-id="c857e-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c857e-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

### <a name="response"></a><span data-ttu-id="c857e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c857e-136">Response</span></span>
<span data-ttu-id="c857e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c857e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




