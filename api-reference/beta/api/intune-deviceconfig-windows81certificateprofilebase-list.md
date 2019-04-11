---
title: Listar windows81CertificateProfileBases
description: Listar Propriedades e relações dos objetos windows81CertificateProfileBase.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b3becbc01cd0e9804bde108536ce5e7b0c1c485e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31804771"
---
# <a name="list-windows81certificateprofilebases"></a><span data-ttu-id="571c9-103">Listar windows81CertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="571c9-103">List windows81CertificateProfileBases</span></span>

> <span data-ttu-id="571c9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="571c9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="571c9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="571c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="571c9-106">Listar Propriedades e relações dos objetos [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="571c9-106">List properties and relationships of the [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="571c9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="571c9-107">Prerequisites</span></span>
<span data-ttu-id="571c9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="571c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="571c9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="571c9-110">Permission type</span></span>|<span data-ttu-id="571c9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="571c9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="571c9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="571c9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="571c9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="571c9-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="571c9-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="571c9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="571c9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="571c9-115">Not supported.</span></span>|
|<span data-ttu-id="571c9-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="571c9-116">Application</span></span>|<span data-ttu-id="571c9-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="571c9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="571c9-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="571c9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="571c9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="571c9-119">Request headers</span></span>
|<span data-ttu-id="571c9-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="571c9-120">Header</span></span>|<span data-ttu-id="571c9-121">Valor</span><span class="sxs-lookup"><span data-stu-id="571c9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="571c9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="571c9-122">Authorization</span></span>|<span data-ttu-id="571c9-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="571c9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="571c9-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="571c9-124">Accept</span></span>|<span data-ttu-id="571c9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="571c9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="571c9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="571c9-126">Request body</span></span>
<span data-ttu-id="571c9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="571c9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="571c9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="571c9-128">Response</span></span>
<span data-ttu-id="571c9-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="571c9-129">If successful, this method returns a `200 OK` response code and a collection of [windows81CertificateProfileBase](../resources/intune-deviceconfig-windows81certificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="571c9-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="571c9-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="571c9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="571c9-131">Request</span></span>
<span data-ttu-id="571c9-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="571c9-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="571c9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="571c9-133">Response</span></span>
<span data-ttu-id="571c9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="571c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1243

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81CertificateProfileBase",
      "id": "61cae8b8-e8b8-61ca-b8e8-ca61b8e8ca61",
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
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "customSubjectAlternativeNames": [
        {
          "@odata.type": "microsoft.graph.customSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ]
    }
  ]
}
```





