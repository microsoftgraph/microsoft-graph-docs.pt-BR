---
title: Lista iosImportedPFXCertificateProfiles
description: Lista as propriedades e os relacionamentos dos objetos iosImportedPFXCertificateProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dd9d808ce55fb1cd050c89a52bae2e48c63ed789
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424340"
---
# <a name="list-iosimportedpfxcertificateprofiles"></a><span data-ttu-id="b10f8-103">Lista iosImportedPFXCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="b10f8-103">List iosImportedPFXCertificateProfiles</span></span>

> <span data-ttu-id="b10f8-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b10f8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b10f8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b10f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b10f8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b10f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b10f8-107">Lista as propriedades e os relacionamentos dos objetos [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="b10f8-107">List properties and relationships of the [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b10f8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b10f8-108">Prerequisites</span></span>
<span data-ttu-id="b10f8-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="b10f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b10f8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b10f8-111">Permission type</span></span>|<span data-ttu-id="b10f8-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b10f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b10f8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b10f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b10f8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b10f8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b10f8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b10f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b10f8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b10f8-116">Not supported.</span></span>|
|<span data-ttu-id="b10f8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b10f8-117">Application</span></span>|<span data-ttu-id="b10f8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b10f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b10f8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b10f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b10f8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b10f8-120">Request headers</span></span>
|<span data-ttu-id="b10f8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b10f8-121">Header</span></span>|<span data-ttu-id="b10f8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b10f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b10f8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b10f8-123">Authorization</span></span>|<span data-ttu-id="b10f8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b10f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b10f8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b10f8-125">Accept</span></span>|<span data-ttu-id="b10f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b10f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b10f8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b10f8-127">Request body</span></span>
<span data-ttu-id="b10f8-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b10f8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b10f8-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b10f8-129">Response</span></span>
<span data-ttu-id="b10f8-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b10f8-130">If successful, this method returns a `200 OK` response code and a collection of [iosImportedPFXCertificateProfile](../resources/intune-deviceconfig-iosimportedpfxcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b10f8-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b10f8-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b10f8-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b10f8-132">Request</span></span>
<span data-ttu-id="b10f8-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b10f8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b10f8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b10f8-134">Response</span></span>
<span data-ttu-id="b10f8-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b10f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 556

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosImportedPFXCertificateProfile",
      "id": "583b9d8c-9d8c-583b-8c9d-3b588c9d3b58",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "intendedPurpose": "smimeEncryption"
    }
  ]
}
```




