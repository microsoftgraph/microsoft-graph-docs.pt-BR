---
title: Excluir deviceManagementDerivedCredentialSettings
description: Exclui um deviceManagementDerivedCredentialSettings.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 063957b79c72bf0fea685e0f4f00997179a79a62
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867501"
---
# <a name="delete-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="c5a2d-103">Excluir deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="c5a2d-103">Delete deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="c5a2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5a2d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5a2d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c5a2d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5a2d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c5a2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a2d-107">Exclui um [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="c5a2d-107">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c5a2d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c5a2d-108">Prerequisites</span></span>
<span data-ttu-id="c5a2d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5a2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5a2d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c5a2d-111">Permission type</span></span>|<span data-ttu-id="c5a2d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c5a2d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5a2d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c5a2d-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="c5a2d-114">&nbsp;&nbsp; **Política de Acesso a Recursos**</span><span class="sxs-lookup"><span data-stu-id="c5a2d-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="c5a2d-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a2d-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c5a2d-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c5a2d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5a2d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c5a2d-117">Not supported.</span></span>|
|<span data-ttu-id="c5a2d-118">Application</span><span class="sxs-lookup"><span data-stu-id="c5a2d-118">Application</span></span>||
|<span data-ttu-id="c5a2d-119">&nbsp;&nbsp; **Política de Acesso a Recursos**</span><span class="sxs-lookup"><span data-stu-id="c5a2d-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="c5a2d-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5a2d-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5a2d-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c5a2d-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="c5a2d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5a2d-122">Request headers</span></span>
|<span data-ttu-id="c5a2d-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c5a2d-123">Header</span></span>|<span data-ttu-id="c5a2d-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c5a2d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5a2d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c5a2d-125">Authorization</span></span>|<span data-ttu-id="c5a2d-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c5a2d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5a2d-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c5a2d-127">Accept</span></span>|<span data-ttu-id="c5a2d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c5a2d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5a2d-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c5a2d-129">Request body</span></span>
<span data-ttu-id="c5a2d-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c5a2d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5a2d-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5a2d-131">Response</span></span>
<span data-ttu-id="c5a2d-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c5a2d-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c5a2d-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c5a2d-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="c5a2d-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c5a2d-134">Request</span></span>
<span data-ttu-id="c5a2d-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c5a2d-135">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

### <a name="response"></a><span data-ttu-id="c5a2d-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c5a2d-136">Response</span></span>
<span data-ttu-id="c5a2d-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c5a2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








