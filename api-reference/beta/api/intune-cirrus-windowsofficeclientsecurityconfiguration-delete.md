---
title: Excluir windowsOfficeClientSecurityConfiguration
description: Exclui uma política de segurança windowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5ac3b985d68fc28e8e9e80bbe495e86f1b75f06c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436666"
---
# <a name="delete-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="4c1ea-103">Excluir windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c1ea-103">Delete windowsOfficeClientSecurityConfiguration</span></span>

<span data-ttu-id="4c1ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c1ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c1ea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c1ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c1ea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c1ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c1ea-107">Exclui uma política de segurança [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="4c1ea-107">Deletes a security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c1ea-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c1ea-108">Prerequisites</span></span>
<span data-ttu-id="4c1ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c1ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c1ea-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c1ea-111">Permission type</span></span>|<span data-ttu-id="4c1ea-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c1ea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c1ea-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c1ea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c1ea-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c1ea-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c1ea-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c1ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c1ea-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c1ea-116">Not supported.</span></span>|
|<span data-ttu-id="4c1ea-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c1ea-117">Application</span></span>|<span data-ttu-id="4c1ea-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c1ea-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c1ea-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c1ea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="4c1ea-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c1ea-120">Request headers</span></span>
|<span data-ttu-id="4c1ea-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c1ea-121">Header</span></span>|<span data-ttu-id="4c1ea-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4c1ea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c1ea-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c1ea-123">Authorization</span></span>|<span data-ttu-id="4c1ea-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c1ea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c1ea-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c1ea-125">Accept</span></span>|<span data-ttu-id="4c1ea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c1ea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c1ea-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c1ea-127">Request body</span></span>
<span data-ttu-id="4c1ea-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4c1ea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c1ea-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c1ea-129">Response</span></span>
<span data-ttu-id="4c1ea-130">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="4c1ea-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4c1ea-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c1ea-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c1ea-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c1ea-132">Request</span></span>
<span data-ttu-id="4c1ea-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c1ea-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="4c1ea-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c1ea-134">Response</span></span>
<span data-ttu-id="4c1ea-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c1ea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



