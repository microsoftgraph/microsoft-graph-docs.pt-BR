---
title: Listar chromeOSOnboardingSettingses
description: Listar propriedades e relações dos objetos chromeOSOnboardingSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f4fc51948be03b084af2105b410b7e63be7af274
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665654"
---
# <a name="list-chromeosonboardingsettingses"></a><span data-ttu-id="b4fa2-103">Listar chromeOSOnboardingSettingses</span><span class="sxs-lookup"><span data-stu-id="b4fa2-103">List chromeOSOnboardingSettingses</span></span>

<span data-ttu-id="b4fa2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4fa2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4fa2-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b4fa2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4fa2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4fa2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4fa2-107">Listar propriedades e relações dos [objetos chromeOSOnboardingSettings.](../resources/intune-chromebooksync-chromeosonboardingsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b4fa2-107">List properties and relationships of the [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4fa2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b4fa2-108">Prerequisites</span></span>
<span data-ttu-id="b4fa2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4fa2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4fa2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b4fa2-111">Permission type</span></span>|<span data-ttu-id="b4fa2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b4fa2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4fa2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b4fa2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4fa2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4fa2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b4fa2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b4fa2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4fa2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b4fa2-116">Not supported.</span></span>|
|<span data-ttu-id="b4fa2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b4fa2-117">Application</span></span>|<span data-ttu-id="b4fa2-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4fa2-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4fa2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b4fa2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/chromeOSOnboardingSettings
```

## <a name="request-headers"></a><span data-ttu-id="b4fa2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b4fa2-120">Request headers</span></span>
|<span data-ttu-id="b4fa2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b4fa2-121">Header</span></span>|<span data-ttu-id="b4fa2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b4fa2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4fa2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b4fa2-123">Authorization</span></span>|<span data-ttu-id="b4fa2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b4fa2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4fa2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b4fa2-125">Accept</span></span>|<span data-ttu-id="b4fa2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4fa2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4fa2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b4fa2-127">Request body</span></span>
<span data-ttu-id="b4fa2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b4fa2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4fa2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4fa2-129">Response</span></span>
<span data-ttu-id="b4fa2-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b4fa2-130">If successful, this method returns a `200 OK` response code and a collection of [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4fa2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b4fa2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4fa2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b4fa2-132">Request</span></span>
<span data-ttu-id="b4fa2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b4fa2-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/chromeOSOnboardingSettings
```

### <a name="response"></a><span data-ttu-id="b4fa2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b4fa2-134">Response</span></span>
<span data-ttu-id="b4fa2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b4fa2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 408

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
      "id": "0344255d-255d-0344-5d25-44035d254403",
      "ownerUserPrincipalName": "Owner User Principal Name value",
      "onboardingStatus": "inprogress",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "lastDirectorySyncDateTime": "2016-12-31T23:57:56.1183185-08:00"
    }
  ]
}
```




