---
title: Excluir targetedManagedAppConfiguration
description: Exclui targetedManagedAppConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 825d18e8833cd98be09a14363dfbbf39eab04b5c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723126"
---
# <a name="delete-targetedmanagedappconfiguration"></a><span data-ttu-id="f1ad0-103">Excluir targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="f1ad0-103">Delete targetedManagedAppConfiguration</span></span>

<span data-ttu-id="f1ad0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1ad0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1ad0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1ad0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1ad0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1ad0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1ad0-107">Exclui [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f1ad0-107">Deletes a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f1ad0-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1ad0-108">Prerequisites</span></span>
<span data-ttu-id="f1ad0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1ad0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1ad0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1ad0-111">Permission type</span></span>|<span data-ttu-id="f1ad0-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1ad0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1ad0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1ad0-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="f1ad0-114">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="f1ad0-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="f1ad0-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ad0-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="f1ad0-116">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="f1ad0-116">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="f1ad0-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ad0-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f1ad0-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1ad0-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1ad0-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1ad0-119">Not supported.</span></span>|
|<span data-ttu-id="f1ad0-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1ad0-120">Application</span></span>||
| <span data-ttu-id="f1ad0-121">&nbsp; &nbsp; **Gerenciamento de aplicativo móvel (GAM)**</span><span class="sxs-lookup"><span data-stu-id="f1ad0-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="f1ad0-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ad0-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="f1ad0-123">&nbsp;&nbsp; **Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="f1ad0-123">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="f1ad0-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1ad0-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1ad0-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1ad0-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f1ad0-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ad0-126">Request headers</span></span>
|<span data-ttu-id="f1ad0-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1ad0-127">Header</span></span>|<span data-ttu-id="f1ad0-128">Valor</span><span class="sxs-lookup"><span data-stu-id="f1ad0-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1ad0-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1ad0-129">Authorization</span></span>|<span data-ttu-id="f1ad0-130">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1ad0-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1ad0-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1ad0-131">Accept</span></span>|<span data-ttu-id="f1ad0-132">application/json</span><span class="sxs-lookup"><span data-stu-id="f1ad0-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1ad0-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ad0-133">Request body</span></span>
<span data-ttu-id="f1ad0-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1ad0-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1ad0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1ad0-135">Response</span></span>
<span data-ttu-id="f1ad0-136">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1ad0-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f1ad0-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1ad0-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f1ad0-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1ad0-138">Request</span></span>
<span data-ttu-id="f1ad0-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1ad0-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="f1ad0-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1ad0-140">Response</span></span>
<span data-ttu-id="f1ad0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1ad0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








