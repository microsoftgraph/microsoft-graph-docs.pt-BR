---
title: Excluir deviceManagementDerivedCredentialSettings
description: Exclui deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bc01aaadd69c7ac6d20756bd75ebe805e8d53e54
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458529"
---
# <a name="delete-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="3b447-103">Excluir deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="3b447-103">Delete deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="3b447-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3b447-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b447-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b447-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b447-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b447-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b447-107">Exclui [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="3b447-107">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b447-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b447-108">Prerequisites</span></span>
<span data-ttu-id="3b447-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b447-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b447-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b447-111">Permission type</span></span>|<span data-ttu-id="3b447-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b447-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b447-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b447-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="3b447-114">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="3b447-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="3b447-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b447-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3b447-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b447-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b447-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b447-117">Not supported.</span></span>|
|<span data-ttu-id="3b447-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b447-118">Application</span></span>||
|<span data-ttu-id="3b447-119">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="3b447-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="3b447-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b447-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b447-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b447-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="3b447-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b447-122">Request headers</span></span>
|<span data-ttu-id="3b447-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b447-123">Header</span></span>|<span data-ttu-id="3b447-124">Valor</span><span class="sxs-lookup"><span data-stu-id="3b447-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b447-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b447-125">Authorization</span></span>|<span data-ttu-id="3b447-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b447-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b447-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b447-127">Accept</span></span>|<span data-ttu-id="3b447-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3b447-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b447-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b447-129">Request body</span></span>
<span data-ttu-id="3b447-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b447-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b447-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b447-131">Response</span></span>
<span data-ttu-id="3b447-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="3b447-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3b447-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b447-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b447-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b447-134">Request</span></span>
<span data-ttu-id="3b447-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b447-135">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

### <a name="response"></a><span data-ttu-id="3b447-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b447-136">Response</span></span>
<span data-ttu-id="3b447-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b447-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









