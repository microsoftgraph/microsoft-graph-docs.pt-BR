---
title: Obter windowsFeatureUpdateProfile
description: Leia as propriedades e as relações do objeto windowsFeatureUpdateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 209d51980ada64c5a42cb34cdd06c58222250b75
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49200593"
---
# <a name="get-windowsfeatureupdateprofile"></a><span data-ttu-id="a0586-103">Obter windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="a0586-103">Get windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="a0586-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0586-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0586-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0586-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0586-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0586-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0586-107">Leia as propriedades e as relações do objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="a0586-107">Read properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0586-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0586-108">Prerequisites</span></span>
<span data-ttu-id="a0586-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0586-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0586-111">Permission type</span></span>|<span data-ttu-id="a0586-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0586-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0586-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0586-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0586-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0586-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a0586-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0586-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0586-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0586-116">Not supported.</span></span>|
|<span data-ttu-id="a0586-117">Application</span><span class="sxs-lookup"><span data-stu-id="a0586-117">Application</span></span>|<span data-ttu-id="a0586-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a0586-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0586-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0586-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0586-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a0586-120">Optional query parameters</span></span>
<span data-ttu-id="a0586-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a0586-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0586-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0586-122">Request headers</span></span>
|<span data-ttu-id="a0586-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0586-123">Header</span></span>|<span data-ttu-id="a0586-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a0586-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0586-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0586-125">Authorization</span></span>|<span data-ttu-id="a0586-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0586-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0586-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0586-127">Accept</span></span>|<span data-ttu-id="a0586-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a0586-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0586-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0586-129">Request body</span></span>
<span data-ttu-id="a0586-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0586-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0586-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0586-131">Response</span></span>
<span data-ttu-id="a0586-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a0586-132">If successful, this method returns a `200 OK` response code and [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0586-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0586-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0586-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0586-134">Request</span></span>
<span data-ttu-id="a0586-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0586-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

### <a name="response"></a><span data-ttu-id="a0586-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0586-136">Response</span></span>
<span data-ttu-id="a0586-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0586-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
    "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
    "displayName": "Display Name value",
    "description": "Description value",
    "featureUpdateVersion": "Feature Update Version value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```




