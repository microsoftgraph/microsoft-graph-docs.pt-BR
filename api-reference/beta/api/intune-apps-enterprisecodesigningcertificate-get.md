---
title: Obter enterpriseCodeSigningCertificate
description: Leia as propriedades e as relações do objeto enterpriseCodeSigningCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c80010ed8a647da334d2a4c9a7b974a99683ad64
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49253002"
---
# <a name="get-enterprisecodesigningcertificate"></a><span data-ttu-id="068c4-103">Obter enterpriseCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="068c4-103">Get enterpriseCodeSigningCertificate</span></span>

<span data-ttu-id="068c4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="068c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="068c4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="068c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="068c4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="068c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="068c4-107">Leia as propriedades e as relações do objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="068c4-107">Read properties and relationships of the [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="068c4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="068c4-108">Prerequisites</span></span>
<span data-ttu-id="068c4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="068c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="068c4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="068c4-111">Permission type</span></span>|<span data-ttu-id="068c4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="068c4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="068c4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="068c4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="068c4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="068c4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="068c4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="068c4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="068c4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="068c4-116">Not supported.</span></span>|
|<span data-ttu-id="068c4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="068c4-117">Application</span></span>|<span data-ttu-id="068c4-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="068c4-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="068c4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="068c4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="068c4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="068c4-120">Optional query parameters</span></span>
<span data-ttu-id="068c4-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="068c4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="068c4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="068c4-122">Request headers</span></span>
|<span data-ttu-id="068c4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="068c4-123">Header</span></span>|<span data-ttu-id="068c4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="068c4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="068c4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="068c4-125">Authorization</span></span>|<span data-ttu-id="068c4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="068c4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="068c4-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="068c4-127">Accept</span></span>|<span data-ttu-id="068c4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="068c4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="068c4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="068c4-129">Request body</span></span>
<span data-ttu-id="068c4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="068c4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="068c4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="068c4-131">Response</span></span>
<span data-ttu-id="068c4-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="068c4-132">If successful, this method returns a `200 OK` response code and [enterpriseCodeSigningCertificate](../resources/intune-apps-enterprisecodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="068c4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="068c4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="068c4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="068c4-134">Request</span></span>
<span data-ttu-id="068c4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="068c4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

### <a name="response"></a><span data-ttu-id="068c4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="068c4-136">Response</span></span>
<span data-ttu-id="068c4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="068c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




