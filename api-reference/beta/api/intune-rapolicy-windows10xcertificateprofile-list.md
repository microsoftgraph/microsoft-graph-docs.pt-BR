---
title: Listar windows10XCertificateProfiles
description: Listar Propriedades e relações dos objetos windows10XCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 79b8653bbba575c61cd1fa36c0d4c212ed1ee5f2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241305"
---
# <a name="list-windows10xcertificateprofiles"></a><span data-ttu-id="3bbbb-103">Listar windows10XCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="3bbbb-103">List windows10XCertificateProfiles</span></span>

<span data-ttu-id="3bbbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bbbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3bbbb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3bbbb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3bbbb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3bbbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3bbbb-107">Listar Propriedades e relações dos objetos [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="3bbbb-107">List properties and relationships of the [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3bbbb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3bbbb-108">Prerequisites</span></span>
<span data-ttu-id="3bbbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3bbbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bbbb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3bbbb-111">Permission type</span></span>|<span data-ttu-id="3bbbb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3bbbb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bbbb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3bbbb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bbbb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bbbb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3bbbb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3bbbb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bbbb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3bbbb-116">Not supported.</span></span>|
|<span data-ttu-id="3bbbb-117">Application</span><span class="sxs-lookup"><span data-stu-id="3bbbb-117">Application</span></span>|<span data-ttu-id="3bbbb-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bbbb-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bbbb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3bbbb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3bbbb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3bbbb-120">Request headers</span></span>
|<span data-ttu-id="3bbbb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3bbbb-121">Header</span></span>|<span data-ttu-id="3bbbb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3bbbb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bbbb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3bbbb-123">Authorization</span></span>|<span data-ttu-id="3bbbb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3bbbb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bbbb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3bbbb-125">Accept</span></span>|<span data-ttu-id="3bbbb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bbbb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bbbb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3bbbb-127">Request body</span></span>
<span data-ttu-id="3bbbb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3bbbb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3bbbb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bbbb-129">Response</span></span>
<span data-ttu-id="3bbbb-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3bbbb-130">If successful, this method returns a `200 OK` response code and a collection of [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bbbb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bbbb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bbbb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bbbb-132">Request</span></span>
<span data-ttu-id="3bbbb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3bbbb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
```

### <a name="response"></a><span data-ttu-id="3bbbb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3bbbb-134">Response</span></span>
<span data-ttu-id="3bbbb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3bbbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




