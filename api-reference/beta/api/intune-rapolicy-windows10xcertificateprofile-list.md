---
title: Listar windows10XCertificateProfiles
description: Listar propriedades e relações dos objetos windows10XCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4df94bcdd7d8ed13d7e6f6016ccb07d7d052f5cf
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151967"
---
# <a name="list-windows10xcertificateprofiles"></a><span data-ttu-id="869c5-103">Listar windows10XCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="869c5-103">List windows10XCertificateProfiles</span></span>

<span data-ttu-id="869c5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="869c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="869c5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="869c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="869c5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="869c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="869c5-107">Listar propriedades e relações dos [objetos windows10XCertificateProfile.](../resources/intune-rapolicy-windows10xcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="869c5-107">List properties and relationships of the [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="869c5-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="869c5-108">Prerequisites</span></span>
<span data-ttu-id="869c5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="869c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="869c5-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="869c5-111">Permission type</span></span>|<span data-ttu-id="869c5-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="869c5-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="869c5-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="869c5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="869c5-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="869c5-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="869c5-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="869c5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="869c5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="869c5-116">Not supported.</span></span>|
|<span data-ttu-id="869c5-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="869c5-117">Application</span></span>|<span data-ttu-id="869c5-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="869c5-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="869c5-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="869c5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="869c5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="869c5-120">Request headers</span></span>
|<span data-ttu-id="869c5-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="869c5-121">Header</span></span>|<span data-ttu-id="869c5-122">Valor</span><span class="sxs-lookup"><span data-stu-id="869c5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="869c5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="869c5-123">Authorization</span></span>|<span data-ttu-id="869c5-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="869c5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="869c5-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="869c5-125">Accept</span></span>|<span data-ttu-id="869c5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="869c5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="869c5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="869c5-127">Request body</span></span>
<span data-ttu-id="869c5-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="869c5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="869c5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="869c5-129">Response</span></span>
<span data-ttu-id="869c5-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="869c5-130">If successful, this method returns a `200 OK` response code and a collection of [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="869c5-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="869c5-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="869c5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="869c5-132">Request</span></span>
<span data-ttu-id="869c5-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="869c5-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
```

### <a name="response"></a><span data-ttu-id="869c5-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="869c5-134">Response</span></span>
<span data-ttu-id="869c5-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="869c5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "value": [
    {
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
  ]
}
```




