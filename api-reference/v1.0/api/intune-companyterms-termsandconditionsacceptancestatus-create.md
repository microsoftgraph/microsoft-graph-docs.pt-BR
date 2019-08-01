---
title: Criar termsAndConditionsAcceptanceStatus
description: Cria um novo objeto termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e30f3e9c844d13c7ee23be818bd001c0f830558
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019818"
---
# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="b03c0-103">Criar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="b03c0-103">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="b03c0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b03c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b03c0-105">Cria um novo objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="b03c0-105">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b03c0-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b03c0-106">Prerequisites</span></span>
<span data-ttu-id="b03c0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b03c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b03c0-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b03c0-109">Permission type</span></span>|<span data-ttu-id="b03c0-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b03c0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b03c0-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b03c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b03c0-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b03c0-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b03c0-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b03c0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b03c0-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b03c0-114">Not supported.</span></span>|
|<span data-ttu-id="b03c0-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b03c0-115">Application</span></span>|<span data-ttu-id="b03c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b03c0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b03c0-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b03c0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="b03c0-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b03c0-118">Request headers</span></span>
|<span data-ttu-id="b03c0-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b03c0-119">Header</span></span>|<span data-ttu-id="b03c0-120">Valor</span><span class="sxs-lookup"><span data-stu-id="b03c0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b03c0-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b03c0-121">Authorization</span></span>|<span data-ttu-id="b03c0-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b03c0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b03c0-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b03c0-123">Accept</span></span>|<span data-ttu-id="b03c0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b03c0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b03c0-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b03c0-125">Request body</span></span>
<span data-ttu-id="b03c0-126">No corpo da solicitação, forneça uma representação JSON do objeto termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="b03c0-126">In the request body, supply a JSON representation for the termsAndConditionsAcceptanceStatus object.</span></span>

<span data-ttu-id="b03c0-127">A tabela a seguir mostra as propriedades que são necessárias ao criar termsAndConditionsAcceptanceStatus.</span><span class="sxs-lookup"><span data-stu-id="b03c0-127">The following table shows the properties that are required when you create the termsAndConditionsAcceptanceStatus.</span></span>

|<span data-ttu-id="b03c0-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b03c0-128">Property</span></span>|<span data-ttu-id="b03c0-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="b03c0-129">Type</span></span>|<span data-ttu-id="b03c0-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="b03c0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b03c0-131">id</span><span class="sxs-lookup"><span data-stu-id="b03c0-131">id</span></span>|<span data-ttu-id="b03c0-132">String</span><span class="sxs-lookup"><span data-stu-id="b03c0-132">String</span></span>|<span data-ttu-id="b03c0-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="b03c0-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="b03c0-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b03c0-134">userDisplayName</span></span>|<span data-ttu-id="b03c0-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b03c0-135">String</span></span>|<span data-ttu-id="b03c0-136">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="b03c0-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="b03c0-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="b03c0-137">acceptedVersion</span></span>|<span data-ttu-id="b03c0-138">Int32</span><span class="sxs-lookup"><span data-stu-id="b03c0-138">Int32</span></span>|<span data-ttu-id="b03c0-139">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b03c0-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="b03c0-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="b03c0-140">acceptedDateTime</span></span>|<span data-ttu-id="b03c0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b03c0-141">DateTimeOffset</span></span>|<span data-ttu-id="b03c0-142">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b03c0-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="b03c0-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b03c0-143">Response</span></span>
<span data-ttu-id="b03c0-144">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b03c0-144">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b03c0-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b03c0-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="b03c0-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b03c0-146">Request</span></span>
<span data-ttu-id="b03c0-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b03c0-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="b03c0-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b03c0-148">Response</span></span>
<span data-ttu-id="b03c0-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b03c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```



