---
title: Listar iosMobileAppConfigurations
description: Lista propriedades e relações dos objetos iosMobileAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c50b9b3c71e3c3dfa5d1481854bf78af0535e054
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144169"
---
# <a name="list-iosmobileappconfigurations"></a><span data-ttu-id="b7b96-103">Listar iosMobileAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="b7b96-103">List iosMobileAppConfigurations</span></span>

<span data-ttu-id="b7b96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7b96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7b96-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b7b96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7b96-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7b96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7b96-107">Lista propriedades e relações dos objetos [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="b7b96-107">List properties and relationships of the [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7b96-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b7b96-108">Prerequisites</span></span>
<span data-ttu-id="b7b96-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7b96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7b96-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b7b96-111">Permission type</span></span>|<span data-ttu-id="b7b96-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b7b96-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7b96-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b7b96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7b96-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b96-114">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b7b96-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b7b96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7b96-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b7b96-116">Not supported.</span></span>|
|<span data-ttu-id="b7b96-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b7b96-117">Application</span></span>|<span data-ttu-id="b7b96-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7b96-118">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7b96-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b7b96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b7b96-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b7b96-120">Request headers</span></span>
|<span data-ttu-id="b7b96-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b7b96-121">Header</span></span>|<span data-ttu-id="b7b96-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b7b96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7b96-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b7b96-123">Authorization</span></span>|<span data-ttu-id="b7b96-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b7b96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7b96-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b7b96-125">Accept</span></span>|<span data-ttu-id="b7b96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7b96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7b96-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b7b96-127">Request body</span></span>
<span data-ttu-id="b7b96-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b7b96-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7b96-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7b96-129">Response</span></span>
<span data-ttu-id="b7b96-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b7b96-130">If successful, this method returns a `200 OK` response code and a collection of [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7b96-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b7b96-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7b96-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b7b96-132">Request</span></span>
<span data-ttu-id="b7b96-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b7b96-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations
```

### <a name="response"></a><span data-ttu-id="b7b96-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b7b96-134">Response</span></span>
<span data-ttu-id="b7b96-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b7b96-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 889

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
      "id": "b2c33191-3191-b2c3-9131-c3b29131c3b2",
      "targetedMobileApps": [
        "Targeted Mobile Apps value"
      ],
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "encodedSettingXml": "ZW5jb2RlZFNldHRpbmdYbWw=",
      "settings": [
        {
          "@odata.type": "microsoft.graph.appConfigurationSettingItem",
          "appConfigKey": "App Config Key value",
          "appConfigKeyType": "integerType",
          "appConfigKeyValue": "App Config Key Value value"
        }
      ]
    }
  ]
}
```




