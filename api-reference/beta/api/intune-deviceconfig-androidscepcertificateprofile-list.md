---
title: Listar androidScepCertificateProfiles
description: Listar Propriedades e relações dos objetos androidScepCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ecca45df51870e3e7e086ba0f37dc9c7014802df
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972589"
---
# <a name="list-androidscepcertificateprofiles"></a><span data-ttu-id="08ce1-103">Listar androidScepCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="08ce1-103">List androidScepCertificateProfiles</span></span>

> <span data-ttu-id="08ce1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08ce1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08ce1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08ce1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08ce1-106">Listar Propriedades e relações dos objetos [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="08ce1-106">List properties and relationships of the [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08ce1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="08ce1-107">Prerequisites</span></span>
<span data-ttu-id="08ce1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08ce1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08ce1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08ce1-110">Permission type</span></span>|<span data-ttu-id="08ce1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="08ce1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08ce1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08ce1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08ce1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="08ce1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="08ce1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08ce1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08ce1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08ce1-115">Not supported.</span></span>|
|<span data-ttu-id="08ce1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08ce1-116">Application</span></span>|<span data-ttu-id="08ce1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08ce1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08ce1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08ce1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="08ce1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08ce1-119">Request headers</span></span>
|<span data-ttu-id="08ce1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="08ce1-120">Header</span></span>|<span data-ttu-id="08ce1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="08ce1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08ce1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="08ce1-122">Authorization</span></span>|<span data-ttu-id="08ce1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="08ce1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08ce1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="08ce1-124">Accept</span></span>|<span data-ttu-id="08ce1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08ce1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08ce1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08ce1-126">Request body</span></span>
<span data-ttu-id="08ce1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="08ce1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08ce1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="08ce1-128">Response</span></span>
<span data-ttu-id="08ce1-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08ce1-129">If successful, this method returns a `200 OK` response code and a collection of [androidScepCertificateProfile](../resources/intune-deviceconfig-androidscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08ce1-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08ce1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="08ce1-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08ce1-131">Request</span></span>
<span data-ttu-id="08ce1-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="08ce1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="08ce1-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="08ce1-133">Response</span></span>
<span data-ttu-id="08ce1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08ce1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidScepCertificateProfile",
      "id": "e9a0dbbd-dbbd-e9a0-bddb-a0e9bddba0e9",
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
      "subjectNameFormat": "commonNameIncludingEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
    }
  ]
}
```




