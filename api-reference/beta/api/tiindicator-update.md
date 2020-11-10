---
title: Atualizar tiIndicator
description: Atualiza as propriedades de um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 16c6becb1009823cf5c9a16cb12ba1b352b82410
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976307"
---
# <a name="update-tiindicator"></a><span data-ttu-id="a5ecf-103">Atualizar tiIndicator</span><span class="sxs-lookup"><span data-stu-id="a5ecf-103">Update tiIndicator</span></span>

<span data-ttu-id="a5ecf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5ecf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5ecf-105">Atualiza as propriedades de um objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="a5ecf-105">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5ecf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5ecf-106">Permissions</span></span>

<span data-ttu-id="a5ecf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5ecf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a5ecf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5ecf-109">Permission type</span></span>                        | <span data-ttu-id="a5ecf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5ecf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a5ecf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5ecf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5ecf-112">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a5ecf-112">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="a5ecf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5ecf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5ecf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-114">Not supported.</span></span> |
| <span data-ttu-id="a5ecf-115">Application</span><span class="sxs-lookup"><span data-stu-id="a5ecf-115">Application</span></span>                            | <span data-ttu-id="a5ecf-116">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="a5ecf-116">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5ecf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5ecf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a5ecf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ecf-118">Request headers</span></span>

| <span data-ttu-id="a5ecf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a5ecf-119">Name</span></span>       | <span data-ttu-id="a5ecf-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5ecf-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a5ecf-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5ecf-121">Authorization</span></span> | <span data-ttu-id="a5ecf-122">Portador {código} **obrigatório**</span><span class="sxs-lookup"><span data-stu-id="a5ecf-122">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="a5ecf-123">Preferir</span><span class="sxs-lookup"><span data-stu-id="a5ecf-123">Prefer</span></span> | <span data-ttu-id="a5ecf-124">Return = representação</span><span class="sxs-lookup"><span data-stu-id="a5ecf-124">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5ecf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ecf-125">Request body</span></span>

<span data-ttu-id="a5ecf-126">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a5ecf-127">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a5ecf-128">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-128">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="a5ecf-129">Os campos obrigatórios são: `id` , `expirationDateTime` , `targetProduct` .</span><span class="sxs-lookup"><span data-stu-id="a5ecf-129">Required fields are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="a5ecf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5ecf-130">Property</span></span>     | <span data-ttu-id="a5ecf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5ecf-131">Type</span></span>        | <span data-ttu-id="a5ecf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5ecf-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a5ecf-133">ação</span><span class="sxs-lookup"><span data-stu-id="a5ecf-133">action</span></span>|<span data-ttu-id="a5ecf-134">string</span><span class="sxs-lookup"><span data-stu-id="a5ecf-134">string</span></span>| <span data-ttu-id="a5ecf-135">A ação a ser aplicada se o indicador for correspondido de dentro da ferramenta de segurança do targetProduct.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-135">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="a5ecf-136">Os valores possíveis são: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-136">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="a5ecf-137">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="a5ecf-137">activityGroupNames</span></span>|<span data-ttu-id="a5ecf-138">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ecf-138">String collection</span></span>|<span data-ttu-id="a5ecf-139">O nome do Cyber Threat Intelligence (s) para as partes responsáveis pela atividade mal-intencionada coberta pelo indicador de ameaças.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-139">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="a5ecf-140">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="a5ecf-140">additionalInformation</span></span>|<span data-ttu-id="a5ecf-141">String</span><span class="sxs-lookup"><span data-stu-id="a5ecf-141">String</span></span>|<span data-ttu-id="a5ecf-142">Uma área catchall na qual os dados extras do indicador não cobertos pelas outras propriedades de tiIndicator podem ser colocados.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-142">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="a5ecf-143">Os dados colocados no additionalInformation normalmente não serão utilizados pela ferramenta de segurança do targetProduct.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-143">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="a5ecf-144">confidence</span><span class="sxs-lookup"><span data-stu-id="a5ecf-144">confidence</span></span>|<span data-ttu-id="a5ecf-145">Int32</span><span class="sxs-lookup"><span data-stu-id="a5ecf-145">Int32</span></span>|<span data-ttu-id="a5ecf-146">Um inteiro representando a confiança dos dados dentro do indicador identifica precisamente o comportamento mal-intencionado.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-146">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="a5ecf-147">Os valores aceitáveis são 0 – 100 com 100 sendo os mais altos.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-147">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="a5ecf-148">description</span><span class="sxs-lookup"><span data-stu-id="a5ecf-148">description</span></span>|<span data-ttu-id="a5ecf-149">String</span><span class="sxs-lookup"><span data-stu-id="a5ecf-149">String</span></span>|<span data-ttu-id="a5ecf-150">Breve descrição (100 caracteres ou menos) da ameaça representada pelo indicador.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-150">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="a5ecf-151">diamondModel</span><span class="sxs-lookup"><span data-stu-id="a5ecf-151">diamondModel</span></span>|[<span data-ttu-id="a5ecf-152">diamondModel</span><span class="sxs-lookup"><span data-stu-id="a5ecf-152">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="a5ecf-153">A área do modelo em losango em que esse indicador existe.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-153">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="a5ecf-154">Os valores possíveis são: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-154">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="a5ecf-155">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a5ecf-155">expirationDateTime</span></span>|<span data-ttu-id="a5ecf-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5ecf-156">DateTimeOffset</span></span>| <span data-ttu-id="a5ecf-157">Cadeia de caracteres DateTime indicando quando o indicador expira.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-157">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="a5ecf-158">Todos os indicadores devem ter uma data de vencimento para evitar indicadores obsoletos persistentes no sistema.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-158">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="a5ecf-159">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-159">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a5ecf-160">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-160">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="a5ecf-161">externalId</span><span class="sxs-lookup"><span data-stu-id="a5ecf-161">externalId</span></span>|<span data-ttu-id="a5ecf-162">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ecf-162">String</span></span>|<span data-ttu-id="a5ecf-163">Um número de identificação que liga o indicador de volta para o sistema do provedor de indicadores (por exemplo, uma chave externa).</span><span class="sxs-lookup"><span data-stu-id="a5ecf-163">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="a5ecf-164">isActive</span><span class="sxs-lookup"><span data-stu-id="a5ecf-164">isActive</span></span>|<span data-ttu-id="a5ecf-165">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5ecf-165">Boolean</span></span>|<span data-ttu-id="a5ecf-166">Usado para desativar indicadores no sistema.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-166">Used to deactivate indicators within system.</span></span> <span data-ttu-id="a5ecf-167">Por padrão, qualquer indicador enviado é definido como ativo.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-167">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="a5ecf-168">No entanto, os provedores podem enviar indicadores existentes com este conjunto como ' false ' para desativar indicadores no sistema.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-168">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="a5ecf-169">killChain</span><span class="sxs-lookup"><span data-stu-id="a5ecf-169">killChain</span></span>|<span data-ttu-id="a5ecf-170">coleção [killChain](#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="a5ecf-170">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="a5ecf-171">Uma matriz JSON de cadeias de caracteres que descreve o ponto ou os pontos na cadeia de Kill que este indicador aponta.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-171">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="a5ecf-172">Consulte "valores de killChain" abaixo para ver os valores exatos.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-172">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="a5ecf-173">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="a5ecf-173">knownFalsePositives</span></span>|<span data-ttu-id="a5ecf-174">String</span><span class="sxs-lookup"><span data-stu-id="a5ecf-174">String</span></span>|<span data-ttu-id="a5ecf-175">Cenários nos quais o indicador pode causar falsos positivos.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-175">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="a5ecf-176">Isso deve ser um texto legível por pessoas.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-176">This should be human-readable text.</span></span>|
|<span data-ttu-id="a5ecf-177">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5ecf-177">lastReportedDateTime</span></span>|<span data-ttu-id="a5ecf-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5ecf-178">DateTimeOffset</span></span>|<span data-ttu-id="a5ecf-179">A última vez que o indicador foi visto.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-179">The last time the indicator was seen.</span></span> <span data-ttu-id="a5ecf-180">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-180">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a5ecf-181">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="a5ecf-181">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="a5ecf-182">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="a5ecf-182">malwareFamilyNames</span></span>|<span data-ttu-id="a5ecf-183">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ecf-183">String collection</span></span>|<span data-ttu-id="a5ecf-184">O nome da família de malware associado a um indicador, se existir.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-184">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="a5ecf-185">A Microsoft prefere o nome da família de malware da Microsoft, se possível, que possa ser encontrado por meio da [enciclopédia de ameaças](https://www.microsoft.com/wdsi/threats)de inteligência de segurança do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-185">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="a5ecf-186">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="a5ecf-186">passiveOnly</span></span>|<span data-ttu-id="a5ecf-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="a5ecf-187">Boolean</span></span>|<span data-ttu-id="a5ecf-188">Determina se o indicador deve acionar um evento que é visível para um usuário final.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-188">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="a5ecf-189">Quando definido como ' true ', as ferramentas de segurança não notificarão o usuário final de que um ' hit ' ocorreu.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-189">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="a5ecf-190">Isso geralmente é tratado como um modo de auditoria ou silencioso por produtos de segurança onde eles simplesmente farão o registro de que uma correspondência ocorreu, mas não executará a ação.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-190">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="a5ecf-191">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-191">Default value is false.</span></span>|
|<span data-ttu-id="a5ecf-192">severity</span><span class="sxs-lookup"><span data-stu-id="a5ecf-192">severity</span></span>|<span data-ttu-id="a5ecf-193">Int32</span><span class="sxs-lookup"><span data-stu-id="a5ecf-193">Int32</span></span>|<span data-ttu-id="a5ecf-194">Um inteiro que representa a gravidade do comportamento mal-intencionado identificado pelos dados dentro do indicador.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-194">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="a5ecf-195">Os valores aceitáveis são 0 – 5, onde 5 é o mais grave e zero não é grave.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-195">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="a5ecf-196">O valor padrão é 3.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-196">Default value is 3.</span></span>|
|<span data-ttu-id="a5ecf-197">tags</span><span class="sxs-lookup"><span data-stu-id="a5ecf-197">tags</span></span>|<span data-ttu-id="a5ecf-198">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5ecf-198">String collection</span></span>|<span data-ttu-id="a5ecf-199">Uma matriz JSON de cadeias de caracteres que armazena marcas arbitrárias/palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-199">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="a5ecf-200">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="a5ecf-200">tlpLevel</span></span>|[<span data-ttu-id="a5ecf-201">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="a5ecf-201">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="a5ecf-202">Valor do protocolo de luz de tráfego para o indicador.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-202">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="a5ecf-203">Os valores possíveis são: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-203">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="a5ecf-204">valores de diamondModel</span><span class="sxs-lookup"><span data-stu-id="a5ecf-204">diamondModel values</span></span>

<span data-ttu-id="a5ecf-205">Para obter informações sobre esse modelo, consulte [o modelo de losango](http://diamondmodel.org).</span><span class="sxs-lookup"><span data-stu-id="a5ecf-205">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="a5ecf-206">Valores</span><span class="sxs-lookup"><span data-stu-id="a5ecf-206">Values</span></span> | <span data-ttu-id="a5ecf-207">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5ecf-207">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="a5ecf-208">adversário</span><span class="sxs-lookup"><span data-stu-id="a5ecf-208">adversary</span></span>|<span data-ttu-id="a5ecf-209">O indicador descreve o adversário.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-209">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="a5ecf-210">função</span><span class="sxs-lookup"><span data-stu-id="a5ecf-210">capability</span></span>|<span data-ttu-id="a5ecf-211">O indicador é uma capacidade do adversário.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-211">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="a5ecf-212">ti</span><span class="sxs-lookup"><span data-stu-id="a5ecf-212">infrastructure</span></span>|<span data-ttu-id="a5ecf-213">O indicador descreve a infraestrutura do adversário.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-213">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="a5ecf-214">vítima</span><span class="sxs-lookup"><span data-stu-id="a5ecf-214">victim</span></span>|<span data-ttu-id="a5ecf-215">O indicador descreve a vítima do adversário.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-215">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="a5ecf-216">valores de killChain</span><span class="sxs-lookup"><span data-stu-id="a5ecf-216">killChain values</span></span>

| <span data-ttu-id="a5ecf-217">Valores</span><span class="sxs-lookup"><span data-stu-id="a5ecf-217">Values</span></span> | <span data-ttu-id="a5ecf-218">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5ecf-218">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="a5ecf-219">Actions</span><span class="sxs-lookup"><span data-stu-id="a5ecf-219">Actions</span></span>|<span data-ttu-id="a5ecf-220">Representa "ações nos objetivos".</span><span class="sxs-lookup"><span data-stu-id="a5ecf-220">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="a5ecf-221">O invasor está aproveitando o sistema comprometido para realizar ações como um ataque de negação de serviço distribuído.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-221">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="a5ecf-222">C2</span><span class="sxs-lookup"><span data-stu-id="a5ecf-222">C2</span></span>|<span data-ttu-id="a5ecf-223">Representa o canal de controle pelo qual um sistema comprometido é manipulado.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-223">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="a5ecf-224">Entrega</span><span class="sxs-lookup"><span data-stu-id="a5ecf-224">Delivery</span></span>|<span data-ttu-id="a5ecf-225">O processo de distribuição do código de exploração para vítimas (por exemplo, USB, email, sites).</span><span class="sxs-lookup"><span data-stu-id="a5ecf-225">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="a5ecf-226">Invasão</span><span class="sxs-lookup"><span data-stu-id="a5ecf-226">Exploitation</span></span>|<span data-ttu-id="a5ecf-227">O código de exploração que aproveita as vulnerabilidades (por exemplo, execução de código).</span><span class="sxs-lookup"><span data-stu-id="a5ecf-227">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="a5ecf-228">Instalação</span><span class="sxs-lookup"><span data-stu-id="a5ecf-228">Installation</span></span>|<span data-ttu-id="a5ecf-229">Instalação de malware após uma vulnerabilidade ter sido explorada.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-229">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="a5ecf-230">Reconhecimento</span><span class="sxs-lookup"><span data-stu-id="a5ecf-230">Reconnaissance</span></span>|<span data-ttu-id="a5ecf-231">O indicador é uma evidência de um grupo de atividades que coleta informações a serem usadas em um ataque futuro.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-231">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="a5ecf-232">Armas</span><span class="sxs-lookup"><span data-stu-id="a5ecf-232">Weaponization</span></span>|<span data-ttu-id="a5ecf-233">Transformar uma vulnerabilidade em código de exploração (por exemplo, malware).</span><span class="sxs-lookup"><span data-stu-id="a5ecf-233">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="a5ecf-234">valores de tlpLevel</span><span class="sxs-lookup"><span data-stu-id="a5ecf-234">tlpLevel values</span></span>

<span data-ttu-id="a5ecf-235">Todos os indicadores devem ter um valor de protocolo de semáforo (TLP) quando ele é enviado.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-235">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="a5ecf-236">Esse valor representa a sensibilidade e o escopo de compartilhamento de um determinado indicador.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-236">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="a5ecf-237">Valores</span><span class="sxs-lookup"><span data-stu-id="a5ecf-237">Values</span></span> | <span data-ttu-id="a5ecf-238">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5ecf-238">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="a5ecf-239">Branco</span><span class="sxs-lookup"><span data-stu-id="a5ecf-239">White</span></span>| <span data-ttu-id="a5ecf-240">Escopo de compartilhamento: ilimitado.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-240">Sharing scope: Unlimited.</span></span> <span data-ttu-id="a5ecf-241">Os indicadores podem ser compartilhados livremente, sem restrição.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-241">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="a5ecf-242">Verde</span><span class="sxs-lookup"><span data-stu-id="a5ecf-242">Green</span></span>| <span data-ttu-id="a5ecf-243">Escopo de compartilhamento: Comunidade.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-243">Sharing scope: Community.</span></span> <span data-ttu-id="a5ecf-244">Os indicadores podem ser compartilhados com a comunidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-244">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="a5ecf-245">Âmbar</span><span class="sxs-lookup"><span data-stu-id="a5ecf-245">Amber</span></span>| <span data-ttu-id="a5ecf-246">Escopo de compartilhamento: limitado.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-246">Sharing scope: Limited.</span></span> <span data-ttu-id="a5ecf-247">Essa é a configuração padrão para indicadores e restringe o compartilhamento apenas àqueles que têm de ser conhecidos: 1) serviços e operadores de serviço que implementam inteligência de ameaças; 2) clientes cujos sistemas apresentam comportamento consistente com o indicador.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-247">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="a5ecf-248">Vermelho</span><span class="sxs-lookup"><span data-stu-id="a5ecf-248">Red</span></span>| <span data-ttu-id="a5ecf-249">Escopo de compartilhamento: pessoal.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-249">Sharing scope: Personal.</span></span> <span data-ttu-id="a5ecf-250">Esses indicadores devem ser compartilhados apenas diretamente e, preferencialmente, em pessoa.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-250">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="a5ecf-251">Normalmente, os indicadores vermelhos do TLP não são incluídos devido às restrições predefinidas.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-251">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="a5ecf-252">Se TLP indicadores vermelhos forem enviados, a propriedade **passiveOnly** também deverá ser definida `True` como.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-252">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="a5ecf-253">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ecf-253">Response</span></span>

<span data-ttu-id="a5ecf-254">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-254">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="a5ecf-255">Se o cabeçalho de solicitação opcional for usado, o método retornará um `200 OK` código de resposta e o objeto [tiIndicator](../resources/tiindicator.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-255">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5ecf-256">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a5ecf-256">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="a5ecf-257">Exemplo 1: solicitação sem cabeçalho de preferência</span><span class="sxs-lookup"><span data-stu-id="a5ecf-257">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="a5ecf-258">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ecf-258">Request</span></span>

<span data-ttu-id="a5ecf-259">Veja a seguir um exemplo da solicitação sem `Prefer` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-259">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="a5ecf-260">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5ecf-260">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[<span data-ttu-id="a5ecf-261">C#</span><span class="sxs-lookup"><span data-stu-id="a5ecf-261">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5ecf-262">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5ecf-262">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5ecf-263">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5ecf-263">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a5ecf-264">Java</span><span class="sxs-lookup"><span data-stu-id="a5ecf-264">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a5ecf-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ecf-265">Response</span></span>

<span data-ttu-id="a5ecf-266">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-266">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="a5ecf-267">Exemplo 2: solicitação com cabeçalho preferencial</span><span class="sxs-lookup"><span data-stu-id="a5ecf-267">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="a5ecf-268">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5ecf-268">Request</span></span>

<span data-ttu-id="a5ecf-269">Veja a seguir um exemplo da solicitação que inclui o `Prefer` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-269">The following is an example of the request that includes the `Prefer` header.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

#### <a name="response"></a><span data-ttu-id="a5ecf-270">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5ecf-270">Response</span></span>

<span data-ttu-id="a5ecf-271">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-271">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="a5ecf-272">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-272">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="a5ecf-273">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5ecf-273">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


