---
title: Listar windows10XSCEPCertificateProfiles
description: Listar Propriedades e relações dos objetos windows10XSCEPCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92cf38cb3557eea1fc7742a6a0726171884dbd61
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241301"
---
# <a name="list-windows10xscepcertificateprofiles"></a><span data-ttu-id="2bdbb-103">Listar windows10XSCEPCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="2bdbb-103">List windows10XSCEPCertificateProfiles</span></span>

<span data-ttu-id="2bdbb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bdbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bdbb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2bdbb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bdbb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bdbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bdbb-107">Listar Propriedades e relações dos objetos [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="2bdbb-107">List properties and relationships of the [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bdbb-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2bdbb-108">Prerequisites</span></span>
<span data-ttu-id="2bdbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bdbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bdbb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bdbb-111">Permission type</span></span>|<span data-ttu-id="2bdbb-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2bdbb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bdbb-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bdbb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2bdbb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bdbb-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2bdbb-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bdbb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bdbb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bdbb-116">Not supported.</span></span>|
|<span data-ttu-id="2bdbb-117">Application</span><span class="sxs-lookup"><span data-stu-id="2bdbb-117">Application</span></span>|<span data-ttu-id="2bdbb-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2bdbb-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bdbb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bdbb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2bdbb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdbb-120">Request headers</span></span>
|<span data-ttu-id="2bdbb-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bdbb-121">Header</span></span>|<span data-ttu-id="2bdbb-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2bdbb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bdbb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bdbb-123">Authorization</span></span>|<span data-ttu-id="2bdbb-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bdbb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bdbb-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2bdbb-125">Accept</span></span>|<span data-ttu-id="2bdbb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2bdbb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bdbb-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdbb-127">Request body</span></span>
<span data-ttu-id="2bdbb-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bdbb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bdbb-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bdbb-129">Response</span></span>
<span data-ttu-id="2bdbb-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bdbb-130">If successful, this method returns a `200 OK` response code and a collection of [windows10XSCEPCertificateProfile](../resources/intune-rapolicy-windows10xscepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bdbb-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bdbb-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bdbb-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bdbb-132">Request</span></span>
<span data-ttu-id="2bdbb-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bdbb-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
```

### <a name="response"></a><span data-ttu-id="2bdbb-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bdbb-134">Response</span></span>
<span data-ttu-id="2bdbb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bdbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1480

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10XSCEPCertificateProfile",
      "id": "d174d58e-d58e-d174-8ed5-74d18ed574d1",
      "version": 7,
      "displayName": "Display Name value",
      "description": "Description value",
      "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "certificateStore": "machine",
      "certificateValidityPeriodScale": "months",
      "certificateValidityPeriodValue": 14,
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ],
      "hashAlgorithm": [
        "sha2"
      ],
      "keySize": "size2048",
      "keyStorageProvider": "useTpmKspOtherwiseFail",
      "keyUsage": "digitalSignature",
      "renewalThresholdPercentage": 10,
      "rootCertificateId": "ed919bbc-9bbc-ed91-bc9b-91edbc9b91ed",
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectAlternativeNameFormats": [
        {
          "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName",
          "sanType": "emailAddress",
          "name": "Name value"
        }
      ],
      "subjectNameFormatString": "Subject Name Format String value"
    }
  ]
}
```




