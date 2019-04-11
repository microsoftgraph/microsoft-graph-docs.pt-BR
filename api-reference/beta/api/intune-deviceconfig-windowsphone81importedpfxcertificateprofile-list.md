---
title: Listar windowsPhone81ImportedPFXCertificateProfiles
description: Listar Propriedades e relações dos objetos windowsPhone81ImportedPFXCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 935cdc6697156e5105cacc38eb1764a12ed73852
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780228"
---
# <a name="list-windowsphone81importedpfxcertificateprofiles"></a><span data-ttu-id="ff134-103">Listar windowsPhone81ImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="ff134-103">List windowsPhone81ImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="ff134-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff134-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff134-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff134-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff134-106">Listar Propriedades e relações dos objetos [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ff134-106">List properties and relationships of the [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff134-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff134-107">Prerequisites</span></span>
<span data-ttu-id="ff134-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff134-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff134-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ff134-110">Permission type</span></span>|<span data-ttu-id="ff134-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ff134-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff134-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ff134-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff134-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff134-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ff134-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ff134-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff134-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff134-115">Not supported.</span></span>|
|<span data-ttu-id="ff134-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff134-116">Application</span></span>|<span data-ttu-id="ff134-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ff134-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff134-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff134-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ff134-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff134-119">Request headers</span></span>
|<span data-ttu-id="ff134-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ff134-120">Header</span></span>|<span data-ttu-id="ff134-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ff134-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff134-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff134-122">Authorization</span></span>|<span data-ttu-id="ff134-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff134-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff134-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ff134-124">Accept</span></span>|<span data-ttu-id="ff134-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ff134-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff134-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff134-126">Request body</span></span>
<span data-ttu-id="ff134-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff134-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff134-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff134-128">Response</span></span>
<span data-ttu-id="ff134-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff134-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81ImportedPFXCertificateProfile](../resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff134-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff134-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff134-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff134-131">Request</span></span>
<span data-ttu-id="ff134-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff134-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ff134-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff134-133">Response</span></span>
<span data-ttu-id="ff134-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff134-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 868

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81ImportedPFXCertificateProfile",
      "id": "08c7f847-f847-08c7-47f8-c70847f8c708",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "renewalThresholdPercentage": 10,
      "keyStorageProvider": "useTpmKspOtherwiseFail",
      "subjectNameFormat": "commonNameIncludingEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```





