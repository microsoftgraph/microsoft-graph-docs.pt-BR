---
title: Tipo de recurso phoneAuthenticationMethod
description: Uma representação de um telefone registrado para um usuário.
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0cab7a96923f49c77e6d160d68e8746530f8dcf2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964545"
---
# <a name="phoneauthenticationmethod-resource-type"></a><span data-ttu-id="2968c-103">Tipo de recurso phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2968c-103">phoneAuthenticationMethod resource type</span></span>

<span data-ttu-id="2968c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2968c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2968c-105">Uma representação de um telefone registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="2968c-105">A representation of a phone registered to a user.</span></span> <span data-ttu-id="2968c-106">Esse recurso inclui o número de telefone, o tipo de telefone e se o telefone está configurado para o usuário entrar via SMS.</span><span class="sxs-lookup"><span data-stu-id="2968c-106">This resource includes the phone number, the phone type, and whether the phone is configured for the user to sign in via SMS.</span></span>

<span data-ttu-id="2968c-107">Um telefone tem um dos três tipos: celular, celular alternativo ou office.</span><span class="sxs-lookup"><span data-stu-id="2968c-107">A phone has one of three types: mobile, alternate mobile, or office.</span></span> <span data-ttu-id="2968c-108">Um usuário pode ter um número registrado para cada tipo e deve ter um telefone celular antes que um telefone celular alternativo seja adicionado.</span><span class="sxs-lookup"><span data-stu-id="2968c-108">A user can have one number registered for each type, and must have a mobile phone before an alternate mobile phone is added.</span></span> <span data-ttu-id="2968c-109">Ao usar um telefone para autenticação multifafação (MFA) ou redefinição de senha de autoatendência (SSPR), o telefone celular é o padrão e o telefone celular alternativo é o backup.</span><span class="sxs-lookup"><span data-stu-id="2968c-109">When using a phone for multi-factor authentication (MFA) or self-service password reset (SSPR), the mobile phone is the default and the alternate mobile phone is the backup.</span></span> 

<span data-ttu-id="2968c-110">Os telefones celulares podem ser usados para sms e chamadas de voz, dependendo das configurações do locatário.</span><span class="sxs-lookup"><span data-stu-id="2968c-110">Mobile phones can be used for both SMS and voice calls, depending on the tenant settings.</span></span>

<span data-ttu-id="2968c-111">Um telefone do office só pode receber chamadas de voz, não mensagens SMS.</span><span class="sxs-lookup"><span data-stu-id="2968c-111">An office phone can only receive voice calls, not SMS messages.</span></span>

## <a name="methods"></a><span data-ttu-id="2968c-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="2968c-112">Methods</span></span>

| <span data-ttu-id="2968c-113">Método</span><span class="sxs-lookup"><span data-stu-id="2968c-113">Method</span></span>       | <span data-ttu-id="2968c-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2968c-114">Return Type</span></span> | <span data-ttu-id="2968c-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="2968c-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2968c-116">List</span><span class="sxs-lookup"><span data-stu-id="2968c-116">List</span></span>](../api/Authentication-list-phonemethods.md) | [<span data-ttu-id="2968c-117">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2968c-117">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="2968c-118">Leia propriedades e relações de todos os objetos phoneAuthenticationMethod deste usuário.</span><span class="sxs-lookup"><span data-stu-id="2968c-118">Read properties and relationships of all of this user's phoneAuthenticationMethod objects.</span></span> |
| [<span data-ttu-id="2968c-119">Get</span><span class="sxs-lookup"><span data-stu-id="2968c-119">Get</span></span>](../api/phoneauthenticationmethod-get.md) | [<span data-ttu-id="2968c-120">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2968c-120">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="2968c-121">Ler propriedades e relações do objeto phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="2968c-121">Read properties and relationships of phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="2968c-122">Atualização</span><span class="sxs-lookup"><span data-stu-id="2968c-122">Update</span></span>](../api/phoneauthenticationmethod-update.md) | [<span data-ttu-id="2968c-123">phoneAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="2968c-123">phoneAuthenticationMethod</span></span>](phoneauthenticationmethod.md) | <span data-ttu-id="2968c-124">Atualizar o objeto phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="2968c-124">Update phoneAuthenticationMethod object.</span></span> |
| [<span data-ttu-id="2968c-125">Delete</span><span class="sxs-lookup"><span data-stu-id="2968c-125">Delete</span></span>](../api/phoneauthenticationmethod-delete.md) | <span data-ttu-id="2968c-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2968c-126">None</span></span> | <span data-ttu-id="2968c-127">Excluir objeto phoneAuthenticationMethod.</span><span class="sxs-lookup"><span data-stu-id="2968c-127">Delete phoneAuthenticationMethod object.</span></span> |
|[<span data-ttu-id="2968c-128">Desabilitar a assinatura de SMS</span><span class="sxs-lookup"><span data-stu-id="2968c-128">Disable SMS signin</span></span>](../api/phoneauthenticationmethod-disablesmssignin.md)|<span data-ttu-id="2968c-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2968c-129">None</span></span>|<span data-ttu-id="2968c-130">Desativar a assinatura SMS para um usuário.</span><span class="sxs-lookup"><span data-stu-id="2968c-130">Turn off SMS sign-in for a user.</span></span>|
|[<span data-ttu-id="2968c-131">Habilitar a assinatura de SMS</span><span class="sxs-lookup"><span data-stu-id="2968c-131">Enable SMS signin</span></span>](../api/phoneauthenticationmethod-enablesmssignin.md)|<span data-ttu-id="2968c-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2968c-132">None</span></span>|<span data-ttu-id="2968c-133">Ativar a assinatura SMS para um usuário.</span><span class="sxs-lookup"><span data-stu-id="2968c-133">Turn on SMS sign-in for a user.</span></span>|

## <a name="properties"></a><span data-ttu-id="2968c-134">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2968c-134">Properties</span></span>

| <span data-ttu-id="2968c-135">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2968c-135">Property</span></span>     | <span data-ttu-id="2968c-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="2968c-136">Type</span></span>        | <span data-ttu-id="2968c-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="2968c-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2968c-138">id</span><span class="sxs-lookup"><span data-stu-id="2968c-138">id</span></span>|<span data-ttu-id="2968c-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2968c-139">String</span></span>| <span data-ttu-id="2968c-140">O identificador desse telefone registrado para esse usuário.</span><span class="sxs-lookup"><span data-stu-id="2968c-140">The identifier of this phone registered to this user.</span></span> <span data-ttu-id="2968c-141">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2968c-141">Read-only.</span></span> <br/><br/><span data-ttu-id="2968c-142">O valor da id é um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="2968c-142">The value of id is one of the following:</span></span><ul><li><span data-ttu-id="2968c-143">`b6332ec1-7057-4abe-9331-3d72feddfe41` - onde **phoneType** é `alternateMobile` .</span><span class="sxs-lookup"><span data-stu-id="2968c-143">`b6332ec1-7057-4abe-9331-3d72feddfe41` - where **phoneType** is `alternateMobile`.</span></span></li><li><span data-ttu-id="2968c-144">`e37fc753-ff3b-4958-9484-eaa9425c82bc` - onde **phoneType** é `office` .</span><span class="sxs-lookup"><span data-stu-id="2968c-144">`e37fc753-ff3b-4958-9484-eaa9425c82bc` - where **phoneType** is `office`.</span></span></li><li><span data-ttu-id="2968c-145">`3179e48a-750b-4051-897c-87b9720928f7` - onde **phoneType** é `mobile` .</span><span class="sxs-lookup"><span data-stu-id="2968c-145">`3179e48a-750b-4051-897c-87b9720928f7` - where **phoneType** is `mobile`.</span></span></li>|
|<span data-ttu-id="2968c-146">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="2968c-146">phoneNumber</span></span>|<span data-ttu-id="2968c-147">String</span><span class="sxs-lookup"><span data-stu-id="2968c-147">String</span></span>|<span data-ttu-id="2968c-148">O número de telefone para texto ou chamada para autenticação.</span><span class="sxs-lookup"><span data-stu-id="2968c-148">The phone number to text or call for authentication.</span></span> <span data-ttu-id="2968c-149">Os números de telefone usam o formato "+ \<country code\> \<number\> \<extension\> x", com a extensão opcional.</span><span class="sxs-lookup"><span data-stu-id="2968c-149">Phone numbers use the format "+\<country code\> \<number\>x\<extension\>", with extension optional.</span></span> <span data-ttu-id="2968c-150">Por exemplo, +1 5555551234 ou +1 5555551234x123 são válidos.</span><span class="sxs-lookup"><span data-stu-id="2968c-150">For example, +1 5555551234 or +1 5555551234x123 are valid.</span></span> <span data-ttu-id="2968c-151">Os números são rejeitados ao criar/atualizar se não corresponderem ao formato necessário.</span><span class="sxs-lookup"><span data-stu-id="2968c-151">Numbers are rejected when creating/updating if they do not match the required format.</span></span> |
|<span data-ttu-id="2968c-152">phoneType</span><span class="sxs-lookup"><span data-stu-id="2968c-152">phoneType</span></span>|<span data-ttu-id="2968c-153">authenticationPhoneType</span><span class="sxs-lookup"><span data-stu-id="2968c-153">authenticationPhoneType</span></span>|<span data-ttu-id="2968c-154">O tipo deste telefone.</span><span class="sxs-lookup"><span data-stu-id="2968c-154">The type of this phone.</span></span> <span data-ttu-id="2968c-155">Os valores possíveis são: `mobile`, `alternateMobile` ou `office`.</span><span class="sxs-lookup"><span data-stu-id="2968c-155">Possible values are: `mobile`, `alternateMobile`, or `office`.</span></span>|
|<span data-ttu-id="2968c-156">smsSignInState</span><span class="sxs-lookup"><span data-stu-id="2968c-156">smsSignInState</span></span>|<span data-ttu-id="2968c-157">authenticationMethodSignInState</span><span class="sxs-lookup"><span data-stu-id="2968c-157">authenticationMethodSignInState</span></span>|<span data-ttu-id="2968c-158">Se um telefone está pronto para ser usado para entrar no SMS ou não.</span><span class="sxs-lookup"><span data-stu-id="2968c-158">Whether a phone is ready to be used for SMS sign-in or not.</span></span> <span data-ttu-id="2968c-159">Os valores possíveis são: `notSupported` , , , , , ou , `notAllowedByPolicy` `notEnabled` `phoneNumberNotUnique` `ready` `notConfigured` `unknownFutureValue` .</span><span class="sxs-lookup"><span data-stu-id="2968c-159">Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, or `notConfigured`, `unknownFutureValue`.</span></span>|

### <a name="smssigninstate-values"></a><span data-ttu-id="2968c-160">valores smsSignInState</span><span class="sxs-lookup"><span data-stu-id="2968c-160">smsSignInState values</span></span>

<span data-ttu-id="2968c-161">A propriedade de estado de login SMS fornece informações sobre se um número de telefone está ou não pronto para entrar via SMS.</span><span class="sxs-lookup"><span data-stu-id="2968c-161">The SMS sign-in state property gives information about whether or not a phone number is ready to sign in via SMS.</span></span> <span data-ttu-id="2968c-162">A seguir estão os valores possíveis.</span><span class="sxs-lookup"><span data-stu-id="2968c-162">The following are the possible values.</span></span>

|<span data-ttu-id="2968c-163">Valor</span><span class="sxs-lookup"><span data-stu-id="2968c-163">Value</span></span>|<span data-ttu-id="2968c-164">Descrição</span><span class="sxs-lookup"><span data-stu-id="2968c-164">Description</span></span>|
|--------|-----------|
|<span data-ttu-id="2968c-165">notSupported</span><span class="sxs-lookup"><span data-stu-id="2968c-165">notSupported</span></span>|<span data-ttu-id="2968c-166">Não há suporte para entrar primário nesse método de autenticação, por exemplo, a login só pode ser habilitada no número móvel principal de um usuário, não no número alternativo.</span><span class="sxs-lookup"><span data-stu-id="2968c-166">Primary sign-in not supported on this authentication method - for example, sign-in can be enabled only on a user's primary mobile number, not the alternate number.</span></span>|
|<span data-ttu-id="2968c-167">notAllowedByPolicy</span><span class="sxs-lookup"><span data-stu-id="2968c-167">notAllowedByPolicy</span></span>|<span data-ttu-id="2968c-168">Esse usuário não está habilitado pela política para usar esse método como uma assinatura primária.</span><span class="sxs-lookup"><span data-stu-id="2968c-168">This user isn't enabled by policy to use this method as a primary sign-in.</span></span>|
|<span data-ttu-id="2968c-169">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2968c-169">notConfigured</span></span>|<span data-ttu-id="2968c-170">Esse usuário está habilitado pela política para usar esse método como login principal, mas precisa tomar medidas adicionais para configurá-lo.</span><span class="sxs-lookup"><span data-stu-id="2968c-170">This user is enabled by policy to use this method as primary sign-in but needs to take additional action to configure it.</span></span>|
|<span data-ttu-id="2968c-171">phoneNumberNotUnique</span><span class="sxs-lookup"><span data-stu-id="2968c-171">phoneNumberNotUnique</span></span>|<span data-ttu-id="2968c-172">Esse usuário tentou configurar um número de telefone como login principal, mas o número não era exclusivo e não pode ser usado como um nome de login.</span><span class="sxs-lookup"><span data-stu-id="2968c-172">This user attempted to set up a phone number as primary sign-in but the number was not unique and can't be used as a sign-in name.</span></span>|
|<span data-ttu-id="2968c-173">ready</span><span class="sxs-lookup"><span data-stu-id="2968c-173">ready</span></span>|<span data-ttu-id="2968c-174">Esse método de autenticação está pronto para ser usado na login principal.</span><span class="sxs-lookup"><span data-stu-id="2968c-174">This authentication method is ready for use in primary sign-in.</span></span>|
|<span data-ttu-id="2968c-175">notEnabled</span><span class="sxs-lookup"><span data-stu-id="2968c-175">notEnabled</span></span>|<span data-ttu-id="2968c-176">Esse método de login não está habilitado</span><span class="sxs-lookup"><span data-stu-id="2968c-176">This sign-in method is not enabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="2968c-177">Relações</span><span class="sxs-lookup"><span data-stu-id="2968c-177">Relationships</span></span>

<span data-ttu-id="2968c-178">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2968c-178">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2968c-179">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2968c-179">JSON representation</span></span>

<span data-ttu-id="2968c-180">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2968c-180">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phoneAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "phoneNumber": "String",
  "phoneType": "string",
  "smsSignInState": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phoneAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


