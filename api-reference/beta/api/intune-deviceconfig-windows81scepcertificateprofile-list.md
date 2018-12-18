---
title: Lista windows81SCEPCertificateProfiles
description: Lista as propriedades e os relacionamentos dos objetos windows81SCEPCertificateProfile.
author: tfitzmac
ms.openlocfilehash: b9f05ef49cb6e5cc5f347c419595276ce8164cdf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304497"
---
# <a name="list-windows81scepcertificateprofiles"></a><span data-ttu-id="0ccc8-103">Lista windows81SCEPCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="0ccc8-103">List windows81SCEPCertificateProfiles</span></span>

> <span data-ttu-id="0ccc8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ccc8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ccc8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ccc8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ccc8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0ccc8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ccc8-107">Lista as propriedades e os relacionamentos dos objetos [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0ccc8-107">List properties and relationships of the [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ccc8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ccc8-108">Prerequisites</span></span>
<span data-ttu-id="0ccc8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ccc8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ccc8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ccc8-111">Permission type</span></span>|<span data-ttu-id="0ccc8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ccc8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ccc8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ccc8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ccc8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ccc8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="0ccc8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ccc8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ccc8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ccc8-116">Not supported.</span></span>|
|<span data-ttu-id="0ccc8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ccc8-117">Application</span></span>|<span data-ttu-id="0ccc8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ccc8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ccc8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ccc8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0ccc8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ccc8-120">Request headers</span></span>
|<span data-ttu-id="0ccc8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ccc8-121">Header</span></span>|<span data-ttu-id="0ccc8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0ccc8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ccc8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ccc8-123">Authorization</span></span>|<span data-ttu-id="0ccc8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ccc8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ccc8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ccc8-125">Accept</span></span>|<span data-ttu-id="0ccc8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ccc8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ccc8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ccc8-127">Request body</span></span>
<span data-ttu-id="0ccc8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ccc8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ccc8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ccc8-129">Response</span></span>
<span data-ttu-id="0ccc8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ccc8-130">If successful, this method returns a `200 OK` response code and a collection of [windows81SCEPCertificateProfile](../resources/intune-deviceconfig-windows81scepcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ccc8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ccc8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ccc8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ccc8-132">Request</span></span>
<span data-ttu-id="0ccc8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ccc8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0ccc8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ccc8-134">Response</span></span>
<span data-ttu-id="0ccc8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ccc8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1616

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows81SCEPCertificateProfile",
      "id": "2daf8af2-8af2-2daf-f28a-af2df28aaf2d",
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
      ],
      "scepServerUrls": [
        "Scep Server Urls value"
      ],
      "subjectNameFormatString": "Subject Name Format String value",
      "keyUsage": "digitalSignature",
      "keySize": "size2048",
      "hashAlgorithm": "sha2",
      "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
      "certificateStore": "machine"
    }
  ]
}
```





