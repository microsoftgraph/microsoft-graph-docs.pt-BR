---
title: Lista androidTrustedRootCertificates
description: Lista as propriedades e os relacionamentos dos objetos androidTrustedRootCertificate.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 35fc14ebc044164e99c0406e1d8f6ca459030f99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854352"
---
# <a name="list-androidtrustedrootcertificates"></a><span data-ttu-id="cfe15-103">Lista androidTrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="cfe15-103">List androidTrustedRootCertificates</span></span>

> <span data-ttu-id="cfe15-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cfe15-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfe15-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cfe15-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfe15-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cfe15-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cfe15-107">Lista as propriedades e os relacionamentos dos objetos [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="cfe15-107">List properties and relationships of the [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cfe15-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cfe15-108">Prerequisites</span></span>
<span data-ttu-id="cfe15-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfe15-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfe15-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfe15-111">Permission type</span></span>|<span data-ttu-id="cfe15-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cfe15-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfe15-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfe15-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cfe15-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="cfe15-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="cfe15-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfe15-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfe15-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfe15-116">Not supported.</span></span>|
|<span data-ttu-id="cfe15-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfe15-117">Application</span></span>|<span data-ttu-id="cfe15-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfe15-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfe15-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfe15-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="cfe15-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe15-120">Request headers</span></span>
|<span data-ttu-id="cfe15-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cfe15-121">Header</span></span>|<span data-ttu-id="cfe15-122">Valor</span><span class="sxs-lookup"><span data-stu-id="cfe15-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfe15-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfe15-123">Authorization</span></span>|<span data-ttu-id="cfe15-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfe15-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfe15-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cfe15-125">Accept</span></span>|<span data-ttu-id="cfe15-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cfe15-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfe15-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe15-127">Request body</span></span>
<span data-ttu-id="cfe15-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cfe15-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cfe15-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfe15-129">Response</span></span>
<span data-ttu-id="cfe15-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfe15-130">If successful, this method returns a `200 OK` response code and a collection of [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfe15-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfe15-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cfe15-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfe15-132">Request</span></span>
<span data-ttu-id="cfe15-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cfe15-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="cfe15-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfe15-134">Response</span></span>
<span data-ttu-id="cfe15-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfe15-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidTrustedRootCertificate",
      "id": "7f8d751e-751e-7f8d-1e75-8d7f1e758d7f",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
      "certFileName": "Cert File Name value"
    }
  ]
}
```





