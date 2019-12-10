---
title: Obter symantecCodeSigningCertificate
description: Leia as propriedades e as relações do objeto symantecCodeSigningCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 53faba19f65dfb37b52a3c416dd96398046ac4bb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39934459"
---
# <a name="get-symanteccodesigningcertificate"></a><span data-ttu-id="03bdc-103">Obter symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="03bdc-103">Get symantecCodeSigningCertificate</span></span>

> <span data-ttu-id="03bdc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03bdc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03bdc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03bdc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03bdc-106">Leia as propriedades e as relações do objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="03bdc-106">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03bdc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="03bdc-107">Prerequisites</span></span>
<span data-ttu-id="03bdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03bdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03bdc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03bdc-110">Permission type</span></span>|<span data-ttu-id="03bdc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="03bdc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03bdc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03bdc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03bdc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="03bdc-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="03bdc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03bdc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03bdc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03bdc-115">Not supported.</span></span>|
|<span data-ttu-id="03bdc-116">Application</span><span class="sxs-lookup"><span data-stu-id="03bdc-116">Application</span></span>|<span data-ttu-id="03bdc-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="03bdc-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03bdc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03bdc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="03bdc-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="03bdc-119">Optional query parameters</span></span>
<span data-ttu-id="03bdc-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="03bdc-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="03bdc-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03bdc-121">Request headers</span></span>
|<span data-ttu-id="03bdc-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="03bdc-122">Header</span></span>|<span data-ttu-id="03bdc-123">Valor</span><span class="sxs-lookup"><span data-stu-id="03bdc-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03bdc-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="03bdc-124">Authorization</span></span>|<span data-ttu-id="03bdc-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03bdc-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03bdc-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="03bdc-126">Accept</span></span>|<span data-ttu-id="03bdc-127">application/json</span><span class="sxs-lookup"><span data-stu-id="03bdc-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03bdc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03bdc-128">Request body</span></span>
<span data-ttu-id="03bdc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="03bdc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03bdc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="03bdc-130">Response</span></span>
<span data-ttu-id="03bdc-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03bdc-131">If successful, this method returns a `200 OK` response code and [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03bdc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03bdc-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="03bdc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03bdc-133">Request</span></span>
<span data-ttu-id="03bdc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03bdc-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
```

### <a name="response"></a><span data-ttu-id="03bdc-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="03bdc-135">Response</span></span>
<span data-ttu-id="03bdc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03bdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": {
    "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
    "id": "00ffe83e-e83e-00ff-3ee8-ff003ee8ff00",
    "content": "Y29udGVudA==",
    "status": "provisioned",
    "password": "Password value",
    "subjectName": "Subject Name value",
    "subject": "Subject value",
    "issuerName": "Issuer Name value",
    "issuer": "Issuer value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00"
  }
}
```





