---
title: Ação windowsPrivacyAccessControls
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f81d061a25c945b70b87fc10a6841b79fbe8026
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971791"
---
# <a name="windowsprivacyaccesscontrols-action"></a><span data-ttu-id="6c5f1-103">Ação windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="6c5f1-103">windowsPrivacyAccessControls action</span></span>

> <span data-ttu-id="6c5f1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c5f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c5f1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c5f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c5f1-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6c5f1-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c5f1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6c5f1-107">Prerequisites</span></span>
<span data-ttu-id="6c5f1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c5f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c5f1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c5f1-110">Permission type</span></span>|<span data-ttu-id="6c5f1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6c5f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c5f1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c5f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c5f1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c5f1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6c5f1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c5f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c5f1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c5f1-115">Not supported.</span></span>|
|<span data-ttu-id="6c5f1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c5f1-116">Application</span></span>|<span data-ttu-id="6c5f1-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c5f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c5f1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c5f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/windowsPrivacyAccessControls
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/windowsPrivacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="6c5f1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5f1-119">Request headers</span></span>
|<span data-ttu-id="6c5f1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6c5f1-120">Header</span></span>|<span data-ttu-id="6c5f1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="6c5f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c5f1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c5f1-122">Authorization</span></span>|<span data-ttu-id="6c5f1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c5f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c5f1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6c5f1-124">Accept</span></span>|<span data-ttu-id="6c5f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c5f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c5f1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5f1-126">Request body</span></span>
<span data-ttu-id="6c5f1-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="6c5f1-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6c5f1-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="6c5f1-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6c5f1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c5f1-129">Property</span></span>|<span data-ttu-id="6c5f1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c5f1-130">Type</span></span>|<span data-ttu-id="6c5f1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c5f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c5f1-132">windowsPrivacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="6c5f1-132">windowsPrivacyAccessControls</span></span>|<span data-ttu-id="6c5f1-133">coleção [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)</span><span class="sxs-lookup"><span data-stu-id="6c5f1-133">[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="6c5f1-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6c5f1-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6c5f1-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5f1-135">Response</span></span>
<span data-ttu-id="6c5f1-136">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6c5f1-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6c5f1-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6c5f1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c5f1-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5f1-138">Request</span></span>
<span data-ttu-id="6c5f1-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c5f1-139">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6c5f1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5f1-140">Response</span></span>
<span data-ttu-id="6c5f1-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c5f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




