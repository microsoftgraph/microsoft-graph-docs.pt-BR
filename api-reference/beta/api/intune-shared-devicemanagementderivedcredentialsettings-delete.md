---
title: Excluir deviceManagementDerivedCredentialSettings
description: Exclui deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b0c215a41fd869637a27cb2987ea9368e81c0795
ms.sourcegitcommit: 0f3e0bd7b57870a0f7b34cf52eaf4776ac82671e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2019
ms.locfileid: "36699450"
---
# <a name="delete-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="1678f-103">Excluir deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="1678f-103">Delete deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="1678f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1678f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1678f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1678f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1678f-106">Exclui [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="1678f-106">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1678f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1678f-107">Prerequisites</span></span>
<span data-ttu-id="1678f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1678f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1678f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1678f-110">Permission type</span></span>|<span data-ttu-id="1678f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1678f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1678f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1678f-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="1678f-113">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="1678f-113">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="1678f-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1678f-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1678f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1678f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1678f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1678f-116">Not supported.</span></span>|
|<span data-ttu-id="1678f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1678f-117">Application</span></span>||
|<span data-ttu-id="1678f-118">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="1678f-118">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="1678f-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1678f-119">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1678f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1678f-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="1678f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1678f-121">Request headers</span></span>
|<span data-ttu-id="1678f-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1678f-122">Header</span></span>|<span data-ttu-id="1678f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="1678f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1678f-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1678f-124">Authorization</span></span>|<span data-ttu-id="1678f-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1678f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1678f-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1678f-126">Accept</span></span>|<span data-ttu-id="1678f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1678f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1678f-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1678f-128">Request body</span></span>
<span data-ttu-id="1678f-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1678f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1678f-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="1678f-130">Response</span></span>
<span data-ttu-id="1678f-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1678f-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1678f-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1678f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1678f-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1678f-133">Request</span></span>
<span data-ttu-id="1678f-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1678f-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

### <a name="response"></a><span data-ttu-id="1678f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1678f-135">Response</span></span>
<span data-ttu-id="1678f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1678f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




