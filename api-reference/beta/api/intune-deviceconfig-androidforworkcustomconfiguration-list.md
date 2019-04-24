---
title: Listar androidForWorkCustomConfigurations
description: Listar Propriedades e relações dos objetos androidForWorkCustomConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 820b75025d550154ac5fa04f77693fb6557de045
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32479299"
---
# <a name="list-androidforworkcustomconfigurations"></a><span data-ttu-id="b0968-103">Listar androidForWorkCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="b0968-103">List androidForWorkCustomConfigurations</span></span>

> <span data-ttu-id="b0968-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0968-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0968-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0968-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0968-106">Listar Propriedades e relações dos objetos [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="b0968-106">List properties and relationships of the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0968-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0968-107">Prerequisites</span></span>
<span data-ttu-id="b0968-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0968-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0968-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0968-110">Permission type</span></span>|<span data-ttu-id="b0968-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0968-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0968-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0968-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0968-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0968-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b0968-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0968-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0968-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0968-115">Not supported.</span></span>|
|<span data-ttu-id="b0968-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0968-116">Application</span></span>|<span data-ttu-id="b0968-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0968-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0968-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0968-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b0968-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0968-119">Request headers</span></span>
|<span data-ttu-id="b0968-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0968-120">Header</span></span>|<span data-ttu-id="b0968-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b0968-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0968-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0968-122">Authorization</span></span>|<span data-ttu-id="b0968-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0968-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0968-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b0968-124">Accept</span></span>|<span data-ttu-id="b0968-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0968-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0968-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0968-126">Request body</span></span>
<span data-ttu-id="b0968-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0968-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0968-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0968-128">Response</span></span>
<span data-ttu-id="b0968-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b0968-129">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0968-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0968-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0968-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0968-131">Request</span></span>
<span data-ttu-id="b0968-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0968-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b0968-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0968-133">Response</span></span>
<span data-ttu-id="b0968-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0968-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 786

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
      "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```





