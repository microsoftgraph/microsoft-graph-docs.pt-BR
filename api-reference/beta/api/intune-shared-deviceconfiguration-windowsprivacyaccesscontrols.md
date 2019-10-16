---
title: Ação windowsPrivacyAccessControls
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d7f5fa6a8928344f9872bc73acaef6f44ad4e042
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537033"
---
# <a name="windowsprivacyaccesscontrols-action"></a><span data-ttu-id="50644-103">Ação windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="50644-103">windowsPrivacyAccessControls action</span></span>

> <span data-ttu-id="50644-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50644-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50644-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50644-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50644-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="50644-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50644-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50644-107">Prerequisites</span></span>
<span data-ttu-id="50644-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50644-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50644-110">Permission type</span></span>|<span data-ttu-id="50644-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50644-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50644-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50644-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="50644-113">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="50644-113">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="50644-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50644-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50644-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50644-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50644-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50644-116">Not supported.</span></span>|
|<span data-ttu-id="50644-117">Application</span><span class="sxs-lookup"><span data-stu-id="50644-117">Application</span></span>||
| <span data-ttu-id="50644-118">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="50644-118">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="50644-119">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50644-119">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50644-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50644-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="50644-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50644-121">Request headers</span></span>
|<span data-ttu-id="50644-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50644-122">Header</span></span>|<span data-ttu-id="50644-123">Valor</span><span class="sxs-lookup"><span data-stu-id="50644-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50644-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="50644-124">Authorization</span></span>|<span data-ttu-id="50644-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50644-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50644-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50644-126">Accept</span></span>|<span data-ttu-id="50644-127">application/json</span><span class="sxs-lookup"><span data-stu-id="50644-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50644-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50644-128">Request body</span></span>
<span data-ttu-id="50644-129">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="50644-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="50644-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="50644-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="50644-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50644-131">Property</span></span>|<span data-ttu-id="50644-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="50644-132">Type</span></span>|<span data-ttu-id="50644-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="50644-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50644-134">windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="50644-134">windowsPrivacyAccessControls</span></span>|<span data-ttu-id="50644-135">coleção [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="50644-135">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="50644-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="50644-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="50644-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="50644-137">Response</span></span>
<span data-ttu-id="50644-138">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="50644-138">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="50644-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50644-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="50644-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50644-140">Request</span></span>
<span data-ttu-id="50644-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50644-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls

Content-type: application/json
Content-length: 379

{
  "windowsPrivacyAccessControls": [
    {
      "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
      "id": "03b15556-5556-03b1-5655-b1035655b103",
      "accessLevel": "forceAllow",
      "dataCategory": "accountInfo",
      "appPackageFamilyName": "App Package Family Name value",
      "appDisplayName": "App Display Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="50644-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="50644-142">Response</span></span>
<span data-ttu-id="50644-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50644-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






