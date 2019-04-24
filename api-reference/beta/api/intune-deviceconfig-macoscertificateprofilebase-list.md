---
title: Listar macOSCertificateProfileBases
description: Listar Propriedades e relações dos objetos macOSCertificateProfileBase.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4227361009e8a214ae42d1e36b35da2f183747f2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518993"
---
# <a name="list-macoscertificateprofilebases"></a><span data-ttu-id="ed414-103">Listar macOSCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="ed414-103">List macOSCertificateProfileBases</span></span>

> <span data-ttu-id="ed414-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed414-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed414-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed414-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed414-106">Listar Propriedades e relações dos objetos [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="ed414-106">List properties and relationships of the [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ed414-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ed414-107">Prerequisites</span></span>
<span data-ttu-id="ed414-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed414-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed414-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed414-110">Permission type</span></span>|<span data-ttu-id="ed414-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ed414-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed414-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed414-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ed414-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ed414-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ed414-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed414-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed414-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed414-115">Not supported.</span></span>|
|<span data-ttu-id="ed414-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed414-116">Application</span></span>|<span data-ttu-id="ed414-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed414-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed414-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed414-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ed414-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed414-119">Request headers</span></span>
|<span data-ttu-id="ed414-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ed414-120">Header</span></span>|<span data-ttu-id="ed414-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ed414-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed414-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed414-122">Authorization</span></span>|<span data-ttu-id="ed414-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ed414-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed414-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ed414-124">Accept</span></span>|<span data-ttu-id="ed414-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ed414-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed414-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed414-126">Request body</span></span>
<span data-ttu-id="ed414-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed414-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed414-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed414-128">Response</span></span>
<span data-ttu-id="ed414-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ed414-129">If successful, this method returns a `200 OK` response code and a collection of [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed414-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ed414-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ed414-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed414-131">Request</span></span>
<span data-ttu-id="ed414-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed414-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ed414-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed414-133">Response</span></span>
<span data-ttu-id="ed414-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ed414-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 745

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCertificateProfileBase",
      "id": "759ed2ad-d2ad-759e-add2-9e75add29e75",
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
      "subjectNameFormat": "commonNameAsEmail",
      "subjectAlternativeNameType": "emailAddress",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months"
    }
  ]
}
```





