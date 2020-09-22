---
title: Excluir deviceManagementDerivedCredentialSettings
description: Exclui deviceManagementDerivedCredentialSettings.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3966e6d456940897d0281f85cad2b00b7b897580
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972018"
---
# <a name="delete-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="57148-103">Excluir deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="57148-103">Delete deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="57148-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57148-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57148-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57148-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57148-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57148-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57148-107">Exclui [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span><span class="sxs-lookup"><span data-stu-id="57148-107">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57148-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57148-108">Prerequisites</span></span>
<span data-ttu-id="57148-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57148-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57148-111">Permission type</span></span>|<span data-ttu-id="57148-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57148-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57148-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57148-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="57148-114">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="57148-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="57148-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57148-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="57148-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57148-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57148-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57148-117">Not supported.</span></span>|
|<span data-ttu-id="57148-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57148-118">Application</span></span>||
|<span data-ttu-id="57148-119">&nbsp;&nbsp; **Política de acesso de recursos**</span><span class="sxs-lookup"><span data-stu-id="57148-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="57148-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57148-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57148-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57148-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="57148-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57148-122">Request headers</span></span>
|<span data-ttu-id="57148-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57148-123">Header</span></span>|<span data-ttu-id="57148-124">Valor</span><span class="sxs-lookup"><span data-stu-id="57148-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57148-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="57148-125">Authorization</span></span>|<span data-ttu-id="57148-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57148-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57148-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57148-127">Accept</span></span>|<span data-ttu-id="57148-128">application/json</span><span class="sxs-lookup"><span data-stu-id="57148-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57148-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57148-129">Request body</span></span>
<span data-ttu-id="57148-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57148-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57148-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="57148-131">Response</span></span>
<span data-ttu-id="57148-132">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="57148-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="57148-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57148-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="57148-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57148-134">Request</span></span>
<span data-ttu-id="57148-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57148-135">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

### <a name="response"></a><span data-ttu-id="57148-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="57148-136">Response</span></span>
<span data-ttu-id="57148-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57148-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```










