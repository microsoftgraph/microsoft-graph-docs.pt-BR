---
title: Obter windows10XCertificateProfile
description: Leia propriedades e relações do objeto windows10XCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a88466fb9a18cb9d44eee8453f57aef594e6488e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152009"
---
# <a name="get-windows10xcertificateprofile"></a><span data-ttu-id="c26ce-103">Obter windows10XCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="c26ce-103">Get windows10XCertificateProfile</span></span>

<span data-ttu-id="c26ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c26ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c26ce-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c26ce-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c26ce-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c26ce-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c26ce-107">Leia propriedades e relações do [objeto windows10XCertificateProfile.](../resources/intune-rapolicy-windows10xcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c26ce-107">Read properties and relationships of the [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c26ce-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c26ce-108">Prerequisites</span></span>
<span data-ttu-id="c26ce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c26ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c26ce-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c26ce-111">Permission type</span></span>|<span data-ttu-id="c26ce-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c26ce-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c26ce-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c26ce-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c26ce-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26ce-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c26ce-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c26ce-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c26ce-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c26ce-116">Not supported.</span></span>|
|<span data-ttu-id="c26ce-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c26ce-117">Application</span></span>|<span data-ttu-id="c26ce-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26ce-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c26ce-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c26ce-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c26ce-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c26ce-120">Optional query parameters</span></span>
<span data-ttu-id="c26ce-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c26ce-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c26ce-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c26ce-122">Request headers</span></span>
|<span data-ttu-id="c26ce-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c26ce-123">Header</span></span>|<span data-ttu-id="c26ce-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c26ce-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c26ce-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c26ce-125">Authorization</span></span>|<span data-ttu-id="c26ce-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c26ce-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c26ce-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c26ce-127">Accept</span></span>|<span data-ttu-id="c26ce-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c26ce-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c26ce-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c26ce-129">Request body</span></span>
<span data-ttu-id="c26ce-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c26ce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c26ce-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c26ce-131">Response</span></span>
<span data-ttu-id="c26ce-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c26ce-132">If successful, this method returns a `200 OK` response code and [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c26ce-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c26ce-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c26ce-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c26ce-134">Request</span></span>
<span data-ttu-id="c26ce-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c26ce-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

### <a name="response"></a><span data-ttu-id="c26ce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c26ce-136">Response</span></span>
<span data-ttu-id="c26ce-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c26ce-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10XCertificateProfile",
    "id": "a11174a1-74a1-a111-a174-11a1a17411a1",
    "version": 7,
    "displayName": "Display Name value",
    "description": "Description value",
    "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




