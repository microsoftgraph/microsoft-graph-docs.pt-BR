---
title: Obter symantecCodeSigningCertificate
description: Leia as propriedades e as relações do objeto symantecCodeSigningCertificate.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ba7f979f43fb107569e35347a023fe1840693c6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43404037"
---
# <a name="get-symanteccodesigningcertificate"></a><span data-ttu-id="642a8-103">Obter symantecCodeSigningCertificate</span><span class="sxs-lookup"><span data-stu-id="642a8-103">Get symantecCodeSigningCertificate</span></span>

<span data-ttu-id="642a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="642a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="642a8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="642a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="642a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="642a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="642a8-107">Leia as propriedades e as relações do objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="642a8-107">Read properties and relationships of the [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="642a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="642a8-108">Prerequisites</span></span>
<span data-ttu-id="642a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="642a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="642a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="642a8-111">Permission type</span></span>|<span data-ttu-id="642a8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="642a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="642a8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="642a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="642a8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="642a8-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="642a8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="642a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="642a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="642a8-116">Not supported.</span></span>|
|<span data-ttu-id="642a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="642a8-117">Application</span></span>|<span data-ttu-id="642a8-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="642a8-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="642a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="642a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/symantecCodeSigningCertificate
```

## <a name="optional-query-parameters"></a><span data-ttu-id="642a8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="642a8-120">Optional query parameters</span></span>
<span data-ttu-id="642a8-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="642a8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="642a8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="642a8-122">Request headers</span></span>
|<span data-ttu-id="642a8-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="642a8-123">Header</span></span>|<span data-ttu-id="642a8-124">Valor</span><span class="sxs-lookup"><span data-stu-id="642a8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="642a8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="642a8-125">Authorization</span></span>|<span data-ttu-id="642a8-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="642a8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="642a8-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="642a8-127">Accept</span></span>|<span data-ttu-id="642a8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="642a8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="642a8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="642a8-129">Request body</span></span>
<span data-ttu-id="642a8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="642a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="642a8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="642a8-131">Response</span></span>
<span data-ttu-id="642a8-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="642a8-132">If successful, this method returns a `200 OK` response code and [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="642a8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="642a8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="642a8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="642a8-134">Request</span></span>
<span data-ttu-id="642a8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="642a8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/symantecCodeSigningCertificate
```

### <a name="response"></a><span data-ttu-id="642a8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="642a8-136">Response</span></span>
<span data-ttu-id="642a8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="642a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



