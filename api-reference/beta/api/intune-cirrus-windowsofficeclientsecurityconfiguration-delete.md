---
title: Excluir windowsOfficeClientSecurityConfiguration
description: Exclui uma política de segurança windowsOfficeClientSecurityConfiguration.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c4e5c03814b4e9663cce1ef12d955bf034d70b2c
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666760"
---
# <a name="delete-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="12713-103">Excluir windowsOfficeClientSecurityConfiguration</span><span class="sxs-lookup"><span data-stu-id="12713-103">Delete windowsOfficeClientSecurityConfiguration</span></span>

<span data-ttu-id="12713-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12713-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12713-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12713-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12713-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12713-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12713-107">Exclui uma política de [segurança windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="12713-107">Deletes a security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12713-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12713-108">Prerequisites</span></span>
<span data-ttu-id="12713-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12713-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12713-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12713-111">Permission type</span></span>|<span data-ttu-id="12713-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12713-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12713-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12713-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12713-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12713-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12713-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12713-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12713-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12713-116">Not supported.</span></span>|
|<span data-ttu-id="12713-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12713-117">Application</span></span>|<span data-ttu-id="12713-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12713-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12713-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12713-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="12713-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12713-120">Request headers</span></span>
|<span data-ttu-id="12713-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12713-121">Header</span></span>|<span data-ttu-id="12713-122">Valor</span><span class="sxs-lookup"><span data-stu-id="12713-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12713-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="12713-123">Authorization</span></span>|<span data-ttu-id="12713-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12713-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12713-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12713-125">Accept</span></span>|<span data-ttu-id="12713-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12713-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12713-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12713-127">Request body</span></span>
<span data-ttu-id="12713-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12713-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12713-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="12713-129">Response</span></span>
<span data-ttu-id="12713-130">Se tiver êxito, este método retornará um código de resposta `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="12713-130">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="12713-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12713-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="12713-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12713-132">Request</span></span>
<span data-ttu-id="12713-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12713-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="12713-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="12713-134">Response</span></span>
<span data-ttu-id="12713-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12713-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```




