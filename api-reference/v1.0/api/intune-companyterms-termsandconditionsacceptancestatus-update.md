---
title: Atualizar termsAndConditionsAcceptanceStatus
description: Atualizar as propriedades de um objeto termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 77dd0941670719f960b5388a86a8143c379bdb5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805814"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="dba3a-103">Atualizar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="dba3a-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="dba3a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dba3a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dba3a-105">Atualizar as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dba3a-105">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dba3a-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dba3a-106">Prerequisites</span></span>
<span data-ttu-id="dba3a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dba3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dba3a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dba3a-109">Permission type</span></span>|<span data-ttu-id="dba3a-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dba3a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dba3a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dba3a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dba3a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dba3a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="dba3a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dba3a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dba3a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dba3a-114">Not supported.</span></span>|
|<span data-ttu-id="dba3a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dba3a-115">Application</span></span>|<span data-ttu-id="dba3a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dba3a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dba3a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dba3a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="dba3a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dba3a-118">Request headers</span></span>
|<span data-ttu-id="dba3a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dba3a-119">Header</span></span>|<span data-ttu-id="dba3a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="dba3a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dba3a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="dba3a-121">Authorization</span></span>|<span data-ttu-id="dba3a-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dba3a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dba3a-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dba3a-123">Accept</span></span>|<span data-ttu-id="dba3a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dba3a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dba3a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dba3a-125">Request body</span></span>
<span data-ttu-id="dba3a-126">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dba3a-126">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="dba3a-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="dba3a-127">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="dba3a-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dba3a-128">Property</span></span>|<span data-ttu-id="dba3a-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="dba3a-129">Type</span></span>|<span data-ttu-id="dba3a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="dba3a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dba3a-131">id</span><span class="sxs-lookup"><span data-stu-id="dba3a-131">id</span></span>|<span data-ttu-id="dba3a-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dba3a-132">String</span></span>|<span data-ttu-id="dba3a-133">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="dba3a-133">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="dba3a-134">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="dba3a-134">userDisplayName</span></span>|<span data-ttu-id="dba3a-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dba3a-135">String</span></span>|<span data-ttu-id="dba3a-136">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="dba3a-136">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="dba3a-137">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="dba3a-137">acceptedVersion</span></span>|<span data-ttu-id="dba3a-138">Int32</span><span class="sxs-lookup"><span data-stu-id="dba3a-138">Int32</span></span>|<span data-ttu-id="dba3a-139">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="dba3a-139">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="dba3a-140">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="dba3a-140">acceptedDateTime</span></span>|<span data-ttu-id="dba3a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dba3a-141">DateTimeOffset</span></span>|<span data-ttu-id="dba3a-142">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="dba3a-142">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="dba3a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="dba3a-143">Response</span></span>
<span data-ttu-id="dba3a-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dba3a-144">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dba3a-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dba3a-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="dba3a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dba3a-146">Request</span></span>
<span data-ttu-id="dba3a-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dba3a-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="dba3a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="dba3a-148">Response</span></span>
<span data-ttu-id="dba3a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dba3a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



