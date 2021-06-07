---
title: Atualizar deviceAppManagement
description: Atualizar as propriedades de um objeto de deviceAppManagement.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a63eb9342f906b6ebf277bfbbb94b52ce0894b5f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748895"
---
# <a name="update-deviceappmanagement"></a><span data-ttu-id="96137-103">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="96137-103">Update deviceAppManagement</span></span>

<span data-ttu-id="96137-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96137-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96137-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96137-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96137-106">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="96137-106">Update the properties of a [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96137-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96137-107">Prerequisites</span></span>
<span data-ttu-id="96137-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96137-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96137-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96137-110">Permission type</span></span>|<span data-ttu-id="96137-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96137-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96137-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96137-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96137-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96137-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="96137-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96137-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96137-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96137-115">Not supported.</span></span>|
|<span data-ttu-id="96137-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96137-116">Application</span></span>|<span data-ttu-id="96137-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96137-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96137-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96137-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="96137-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96137-119">Request headers</span></span>
|<span data-ttu-id="96137-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96137-120">Header</span></span>|<span data-ttu-id="96137-121">Valor</span><span class="sxs-lookup"><span data-stu-id="96137-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96137-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="96137-122">Authorization</span></span>|<span data-ttu-id="96137-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96137-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96137-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96137-124">Accept</span></span>|<span data-ttu-id="96137-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96137-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96137-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96137-126">Request body</span></span>
<span data-ttu-id="96137-127">No corpo da solicitação, forneça uma representação JSON do objeto [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="96137-127">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md) object.</span></span>

<span data-ttu-id="96137-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="96137-128">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md).</span></span>

|<span data-ttu-id="96137-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96137-129">Property</span></span>|<span data-ttu-id="96137-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="96137-130">Type</span></span>|<span data-ttu-id="96137-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="96137-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96137-132">id</span><span class="sxs-lookup"><span data-stu-id="96137-132">id</span></span>|<span data-ttu-id="96137-133">String</span><span class="sxs-lookup"><span data-stu-id="96137-133">String</span></span>|<span data-ttu-id="96137-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="96137-134">Key of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="96137-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="96137-135">Response</span></span>
<span data-ttu-id="96137-136">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96137-136">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune-partnerintegration-deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96137-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96137-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="96137-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96137-138">Request</span></span>
<span data-ttu-id="96137-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96137-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 61

{
  "@odata.type": "#microsoft.graph.deviceAppManagement"
}
```

### <a name="response"></a><span data-ttu-id="96137-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="96137-140">Response</span></span>
<span data-ttu-id="96137-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96137-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```




