---
title: Atualizar ndesConnector
description: Atualize as propriedades de um objeto ndesConnector.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8c78502bb0670eca08b896bf1a0b732f94b669cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418418"
---
# <a name="update-ndesconnector"></a><span data-ttu-id="19fda-103">Atualizar ndesConnector</span><span class="sxs-lookup"><span data-stu-id="19fda-103">Update ndesConnector</span></span>

> <span data-ttu-id="19fda-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="19fda-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="19fda-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="19fda-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19fda-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="19fda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19fda-107">Atualize as propriedades de um objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="19fda-107">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19fda-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="19fda-108">Prerequisites</span></span>
<span data-ttu-id="19fda-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="19fda-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="19fda-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19fda-111">Permission type</span></span>|<span data-ttu-id="19fda-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="19fda-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19fda-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19fda-113">Delegated (work or school account)</span></span>|<span data-ttu-id="19fda-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19fda-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19fda-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19fda-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19fda-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19fda-116">Not supported.</span></span>|
|<span data-ttu-id="19fda-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19fda-117">Application</span></span>|<span data-ttu-id="19fda-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19fda-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19fda-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19fda-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="19fda-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="19fda-120">Request headers</span></span>
|<span data-ttu-id="19fda-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="19fda-121">Header</span></span>|<span data-ttu-id="19fda-122">Valor</span><span class="sxs-lookup"><span data-stu-id="19fda-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19fda-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="19fda-123">Authorization</span></span>|<span data-ttu-id="19fda-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19fda-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19fda-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="19fda-125">Accept</span></span>|<span data-ttu-id="19fda-126">application/json</span><span class="sxs-lookup"><span data-stu-id="19fda-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19fda-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19fda-127">Request body</span></span>
<span data-ttu-id="19fda-128">No corpo da solicitação, fornece uma representação JSON para o objeto [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) .</span><span class="sxs-lookup"><span data-stu-id="19fda-128">In the request body, supply a JSON representation for the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

<span data-ttu-id="19fda-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span><span class="sxs-lookup"><span data-stu-id="19fda-129">The following table shows the properties that are required when you create the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>

|<span data-ttu-id="19fda-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19fda-130">Property</span></span>|<span data-ttu-id="19fda-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="19fda-131">Type</span></span>|<span data-ttu-id="19fda-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="19fda-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19fda-133">id</span><span class="sxs-lookup"><span data-stu-id="19fda-133">id</span></span>|<span data-ttu-id="19fda-134">String</span><span class="sxs-lookup"><span data-stu-id="19fda-134">String</span></span>|<span data-ttu-id="19fda-135">A chave do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="19fda-135">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="19fda-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="19fda-136">lastConnectionDateTime</span></span>|<span data-ttu-id="19fda-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19fda-137">DateTimeOffset</span></span>|<span data-ttu-id="19fda-138">Hora da última conexão para o conector Ndes</span><span class="sxs-lookup"><span data-stu-id="19fda-138">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="19fda-139">estado</span><span class="sxs-lookup"><span data-stu-id="19fda-139">state</span></span>|[<span data-ttu-id="19fda-140">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="19fda-140">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="19fda-141">Status do conector NDES.</span><span class="sxs-lookup"><span data-stu-id="19fda-141">Ndes Connector Status.</span></span> <span data-ttu-id="19fda-142">Os valores possíveis são: `none`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="19fda-142">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="19fda-143">displayName</span><span class="sxs-lookup"><span data-stu-id="19fda-143">displayName</span></span>|<span data-ttu-id="19fda-144">String</span><span class="sxs-lookup"><span data-stu-id="19fda-144">String</span></span>|<span data-ttu-id="19fda-145">O nome amigável do conector Ndes.</span><span class="sxs-lookup"><span data-stu-id="19fda-145">The friendly name of the Ndes Connector.</span></span>|



## <a name="response"></a><span data-ttu-id="19fda-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="19fda-146">Response</span></span>
<span data-ttu-id="19fda-147">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19fda-147">If successful, this method returns a `200 OK` response code and an updated [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19fda-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19fda-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="19fda-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19fda-149">Request</span></span>
<span data-ttu-id="19fda-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19fda-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="19fda-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="19fda-151">Response</span></span>
<span data-ttu-id="19fda-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19fda-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
  "state": "active",
  "displayName": "Display Name value"
}
```




