---
title: Atualizar tiIndicator
description: Atualiza as propriedades de um objeto tiIndicator.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 34c73f3acec6084989f48d7e96b7bc05cbd2b115
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219738"
---
# <a name="update-tiindicator"></a><span data-ttu-id="f798d-103">Atualizar tiIndicator</span><span class="sxs-lookup"><span data-stu-id="f798d-103">Update tiIndicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f798d-104">Atualiza as propriedades de um objeto [tiIndicator](../resources/tiindicator.md) .</span><span class="sxs-lookup"><span data-stu-id="f798d-104">Update the properties of a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f798d-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f798d-105">Permissions</span></span>

<span data-ttu-id="f798d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f798d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f798d-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f798d-108">Permission type</span></span>                        | <span data-ttu-id="f798d-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f798d-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f798d-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f798d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f798d-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f798d-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="f798d-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f798d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f798d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f798d-113">Not supported.</span></span> |
| <span data-ttu-id="f798d-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f798d-114">Application</span></span>                            | <span data-ttu-id="f798d-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="f798d-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="f798d-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f798d-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f798d-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f798d-117">Request headers</span></span>

| <span data-ttu-id="f798d-118">Nome</span><span class="sxs-lookup"><span data-stu-id="f798d-118">Name</span></span>       | <span data-ttu-id="f798d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="f798d-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f798d-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f798d-120">Authorization</span></span> | <span data-ttu-id="f798d-121">Portador {código} **obrigatório**</span><span class="sxs-lookup"><span data-stu-id="f798d-121">Bearer {code} **Required**</span></span> |
|<span data-ttu-id="f798d-122">Preferir</span><span class="sxs-lookup"><span data-stu-id="f798d-122">Prefer</span></span> | <span data-ttu-id="f798d-123">Return = representação</span><span class="sxs-lookup"><span data-stu-id="f798d-123">return=representation</span></span> |

## <a name="request-body"></a><span data-ttu-id="f798d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f798d-124">Request body</span></span>

<span data-ttu-id="f798d-125">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="f798d-125">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="f798d-126">Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade.</span><span class="sxs-lookup"><span data-stu-id="f798d-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="f798d-127">Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="f798d-127">For best performance, don't include existing values that haven't changed.</span></span> <span data-ttu-id="f798d-128">Os campos obrigatórios `id`são `expirationDateTime`: `targetProduct`,,.</span><span class="sxs-lookup"><span data-stu-id="f798d-128">Required fields are: `id`, `expirationDateTime`, `targetProduct`.</span></span>

| <span data-ttu-id="f798d-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f798d-129">Property</span></span>     | <span data-ttu-id="f798d-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f798d-130">Type</span></span>        | <span data-ttu-id="f798d-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f798d-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f798d-132">ação</span><span class="sxs-lookup"><span data-stu-id="f798d-132">action</span></span>|<span data-ttu-id="f798d-133">string</span><span class="sxs-lookup"><span data-stu-id="f798d-133">string</span></span>| <span data-ttu-id="f798d-134">A ação a ser aplicada se o indicador for correspondido de dentro da ferramenta de segurança do targetProduct.</span><span class="sxs-lookup"><span data-stu-id="f798d-134">The action to apply if the indicator is matched from within the targetProduct security tool.</span></span> <span data-ttu-id="f798d-135">Os valores possíveis são: `unknown`, `allow`, `block`, `alert`.</span><span class="sxs-lookup"><span data-stu-id="f798d-135">Possible values are: `unknown`, `allow`, `block`, `alert`.</span></span>|
|<span data-ttu-id="f798d-136">activityGroupNames</span><span class="sxs-lookup"><span data-stu-id="f798d-136">activityGroupNames</span></span>|<span data-ttu-id="f798d-137">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f798d-137">String collection</span></span>|<span data-ttu-id="f798d-138">O nome do Cyber Threat Intelligence (s) para as partes responsáveis pela atividade mal-intencionada coberta pelo indicador de ameaças.</span><span class="sxs-lookup"><span data-stu-id="f798d-138">The cyber threat intelligence name(s) for the parties responsible for the malicious activity covered by the threat indicator.</span></span>|
|<span data-ttu-id="f798d-139">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="f798d-139">additionalInformation</span></span>|<span data-ttu-id="f798d-140">String</span><span class="sxs-lookup"><span data-stu-id="f798d-140">String</span></span>|<span data-ttu-id="f798d-141">Uma área catchall na qual os dados extras do indicador não cobertos pelas outras propriedades de tiIndicator podem ser colocados.</span><span class="sxs-lookup"><span data-stu-id="f798d-141">A catchall area into which extra data from the indicator not covered by the other tiIndicator properties may be placed.</span></span> <span data-ttu-id="f798d-142">Os dados colocados no additionalInformation normalmente não serão utilizados pela ferramenta de segurança do targetProduct.</span><span class="sxs-lookup"><span data-stu-id="f798d-142">Data placed into additionalInformation will typically not be utilized by the targetProduct security tool.</span></span>|
|<span data-ttu-id="f798d-143">confidence</span><span class="sxs-lookup"><span data-stu-id="f798d-143">confidence</span></span>|<span data-ttu-id="f798d-144">Int32</span><span class="sxs-lookup"><span data-stu-id="f798d-144">Int32</span></span>|<span data-ttu-id="f798d-145">Um inteiro representando a confiança dos dados dentro do indicador identifica precisamente o comportamento mal-intencionado.</span><span class="sxs-lookup"><span data-stu-id="f798d-145">An integer representing the confidence the data within the indicator accurately identifies malicious behavior.</span></span> <span data-ttu-id="f798d-146">Os valores aceitáveis são 0 – 100 com 100 sendo os mais altos.</span><span class="sxs-lookup"><span data-stu-id="f798d-146">Acceptable values are 0 – 100 with 100 being the highest.</span></span>|
|<span data-ttu-id="f798d-147">descrição</span><span class="sxs-lookup"><span data-stu-id="f798d-147">description</span></span>|<span data-ttu-id="f798d-148">String</span><span class="sxs-lookup"><span data-stu-id="f798d-148">String</span></span>|<span data-ttu-id="f798d-149">Breve descrição (100 caracteres ou menos) da ameaça representada pelo indicador.</span><span class="sxs-lookup"><span data-stu-id="f798d-149">Brief description (100 characters or less) of the threat represented by the indicator.</span></span>|
|<span data-ttu-id="f798d-150">diamondModel</span><span class="sxs-lookup"><span data-stu-id="f798d-150">diamondModel</span></span>|[<span data-ttu-id="f798d-151">diamondModel</span><span class="sxs-lookup"><span data-stu-id="f798d-151">diamondModel</span></span>](#diamondmodel-values)|<span data-ttu-id="f798d-152">A área do modelo em losango em que esse indicador existe.</span><span class="sxs-lookup"><span data-stu-id="f798d-152">The area of the Diamond Model in which this indicator exists.</span></span> <span data-ttu-id="f798d-153">Os valores possíveis são: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span><span class="sxs-lookup"><span data-stu-id="f798d-153">Possible values are: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.</span></span>|
|<span data-ttu-id="f798d-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f798d-154">expirationDateTime</span></span>|<span data-ttu-id="f798d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f798d-155">DateTimeOffset</span></span>| <span data-ttu-id="f798d-156">Cadeia de caracteres DateTime indicando quando o indicador expira.</span><span class="sxs-lookup"><span data-stu-id="f798d-156">DateTime string indicating when the Indicator expires.</span></span> <span data-ttu-id="f798d-157">Todos os indicadores devem ter uma data de vencimento para evitar indicadores obsoletos persistentes no sistema.</span><span class="sxs-lookup"><span data-stu-id="f798d-157">All indicators must have an expiration date to avoid stale indicators persisting in the system.</span></span> <span data-ttu-id="f798d-158">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f798d-158">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f798d-159">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="f798d-159">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="f798d-160">externalId</span><span class="sxs-lookup"><span data-stu-id="f798d-160">externalId</span></span>|<span data-ttu-id="f798d-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f798d-161">String</span></span>|<span data-ttu-id="f798d-162">Um número de identificação que liga o indicador de volta para o sistema do provedor de indicadores (por exemplo, uma chave externa).</span><span class="sxs-lookup"><span data-stu-id="f798d-162">An identification number that ties the indicator back to the indicator provider’s system (e.g. a foreign key).</span></span>|
|<span data-ttu-id="f798d-163">isActive</span><span class="sxs-lookup"><span data-stu-id="f798d-163">isActive</span></span>|<span data-ttu-id="f798d-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="f798d-164">Boolean</span></span>|<span data-ttu-id="f798d-165">Usado para desativar indicadores no sistema.</span><span class="sxs-lookup"><span data-stu-id="f798d-165">Used to deactivate indicators within system.</span></span> <span data-ttu-id="f798d-166">Por padrão, qualquer indicador enviado é definido como ativo.</span><span class="sxs-lookup"><span data-stu-id="f798d-166">By default, any indicator submitted is set as active.</span></span> <span data-ttu-id="f798d-167">No entanto, os provedores podem enviar indicadores existentes com este conjunto como ' false ' para desativar indicadores no sistema.</span><span class="sxs-lookup"><span data-stu-id="f798d-167">However, providers may submit existing indicators with this set to ‘False’ to deactivate indicators in the system.</span></span>|
|<span data-ttu-id="f798d-168">killChain</span><span class="sxs-lookup"><span data-stu-id="f798d-168">killChain</span></span>|<span data-ttu-id="f798d-169">coleção [killChain](#killchain-values)</span><span class="sxs-lookup"><span data-stu-id="f798d-169">[killChain](#killchain-values) collection</span></span>|<span data-ttu-id="f798d-170">Uma matriz JSON de cadeias de caracteres que descreve o ponto ou os pontos na cadeia de Kill que este indicador aponta.</span><span class="sxs-lookup"><span data-stu-id="f798d-170">A JSON array of strings that describes which point or points on the Kill Chain this indicator targets.</span></span> <span data-ttu-id="f798d-171">Consulte "valores de killChain" abaixo para ver os valores exatos.</span><span class="sxs-lookup"><span data-stu-id="f798d-171">See "killChain values" below for exact values.</span></span>|
|<span data-ttu-id="f798d-172">knownFalsePositives</span><span class="sxs-lookup"><span data-stu-id="f798d-172">knownFalsePositives</span></span>|<span data-ttu-id="f798d-173">String</span><span class="sxs-lookup"><span data-stu-id="f798d-173">String</span></span>|<span data-ttu-id="f798d-174">Cenários nos quais o indicador pode causar falsos positivos.</span><span class="sxs-lookup"><span data-stu-id="f798d-174">Scenarios in which the indicator may cause false positives.</span></span> <span data-ttu-id="f798d-175">Isso deve ser um texto legível por pessoas.</span><span class="sxs-lookup"><span data-stu-id="f798d-175">This should be human-readable text.</span></span>|
|<span data-ttu-id="f798d-176">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="f798d-176">lastReportedDateTime</span></span>|<span data-ttu-id="f798d-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f798d-177">DateTimeOffset</span></span>|<span data-ttu-id="f798d-178">A última vez que o indicador foi visto.</span><span class="sxs-lookup"><span data-stu-id="f798d-178">The last time the indicator was seen.</span></span> <span data-ttu-id="f798d-179">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f798d-179">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f798d-180">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="f798d-180">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="f798d-181">malwareFamilyNames</span><span class="sxs-lookup"><span data-stu-id="f798d-181">malwareFamilyNames</span></span>|<span data-ttu-id="f798d-182">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f798d-182">String collection</span></span>|<span data-ttu-id="f798d-183">O nome da família de malware associado a um indicador, se existir.</span><span class="sxs-lookup"><span data-stu-id="f798d-183">The malware family name associated with an indicator if it exists.</span></span> <span data-ttu-id="f798d-184">A Microsoft prefere o nome da família de malware da Microsoft, se possível, que possa ser encontrado por meio da [enciclopédia de ameaças](https://www.microsoft.com/wdsi/threats)de inteligência de segurança do Windows Defender.</span><span class="sxs-lookup"><span data-stu-id="f798d-184">Microsoft prefers the Microsoft malware family name if at all possible which can be found via the Windows Defender Security Intelligence [threat encyclopedia](https://www.microsoft.com/wdsi/threats).</span></span>|
|<span data-ttu-id="f798d-185">passiveOnly</span><span class="sxs-lookup"><span data-stu-id="f798d-185">passiveOnly</span></span>|<span data-ttu-id="f798d-186">Booliano</span><span class="sxs-lookup"><span data-stu-id="f798d-186">Boolean</span></span>|<span data-ttu-id="f798d-187">Determina se o indicador deve acionar um evento que é visível para um usuário final.</span><span class="sxs-lookup"><span data-stu-id="f798d-187">Determines if the indicator should trigger an event that is visible to an end-user.</span></span> <span data-ttu-id="f798d-188">Quando definido como ' true ', as ferramentas de segurança não notificarão o usuário final de que um ' hit ' ocorreu.</span><span class="sxs-lookup"><span data-stu-id="f798d-188">When set to ‘true,’ security tools will not notify the end user that a ‘hit’ has occurred.</span></span> <span data-ttu-id="f798d-189">Isso geralmente é tratado como um modo de auditoria ou silencioso por produtos de segurança onde eles simplesmente farão o registro de que uma correspondência ocorreu, mas não executará a ação.</span><span class="sxs-lookup"><span data-stu-id="f798d-189">This is most often treated as audit or silent mode by security products where they will simply log that a match occurred but will not perform the action.</span></span> <span data-ttu-id="f798d-190">O valor padrão é falso.</span><span class="sxs-lookup"><span data-stu-id="f798d-190">Default value is false.</span></span>|
|<span data-ttu-id="f798d-191">severity</span><span class="sxs-lookup"><span data-stu-id="f798d-191">severity</span></span>|<span data-ttu-id="f798d-192">Int32</span><span class="sxs-lookup"><span data-stu-id="f798d-192">Int32</span></span>|<span data-ttu-id="f798d-193">Um inteiro que representa a gravidade do comportamento mal-intencionado identificado pelos dados dentro do indicador.</span><span class="sxs-lookup"><span data-stu-id="f798d-193">An integer representing the severity of the malicious behavior identified by the data within the indicator.</span></span> <span data-ttu-id="f798d-194">Os valores aceitáveis são 0 – 5, onde 5 é o mais grave e zero não é grave.</span><span class="sxs-lookup"><span data-stu-id="f798d-194">Acceptable values are 0 – 5 where 5 is the most severe and zero is not severe at all.</span></span> <span data-ttu-id="f798d-195">O valor padrão é 3.</span><span class="sxs-lookup"><span data-stu-id="f798d-195">Default value is 3.</span></span>|
|<span data-ttu-id="f798d-196">tags</span><span class="sxs-lookup"><span data-stu-id="f798d-196">tags</span></span>|<span data-ttu-id="f798d-197">String collection</span><span class="sxs-lookup"><span data-stu-id="f798d-197">String collection</span></span>|<span data-ttu-id="f798d-198">Uma matriz JSON de cadeias de caracteres que armazena marcas arbitrárias/palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="f798d-198">A JSON array of strings that stores arbitrary tags/keywords.</span></span>|
|<span data-ttu-id="f798d-199">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="f798d-199">tlpLevel</span></span>|[<span data-ttu-id="f798d-200">tlpLevel</span><span class="sxs-lookup"><span data-stu-id="f798d-200">tlpLevel</span></span>](#tlplevel-values)| <span data-ttu-id="f798d-201">Valor do protocolo de luz de tráfego para o indicador.</span><span class="sxs-lookup"><span data-stu-id="f798d-201">Traffic Light Protocol value for the indicator.</span></span> <span data-ttu-id="f798d-202">Os valores possíveis são: `unknown`, `white`, `green`, `amber`, `red`.</span><span class="sxs-lookup"><span data-stu-id="f798d-202">Possible values are: `unknown`, `white`, `green`, `amber`, `red`.</span></span>|

### <a name="diamondmodel-values"></a><span data-ttu-id="f798d-203">valores de diamondModel</span><span class="sxs-lookup"><span data-stu-id="f798d-203">diamondModel values</span></span>

<span data-ttu-id="f798d-204">Para obter informações sobre esse modelo, consulte [o modelo de losango](http://diamondmodel.org).</span><span class="sxs-lookup"><span data-stu-id="f798d-204">For information about this model, see [The diamond model](http://diamondmodel.org).</span></span>

| <span data-ttu-id="f798d-205">Valores</span><span class="sxs-lookup"><span data-stu-id="f798d-205">Values</span></span> | <span data-ttu-id="f798d-206">Descrição</span><span class="sxs-lookup"><span data-stu-id="f798d-206">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="f798d-207">adversário</span><span class="sxs-lookup"><span data-stu-id="f798d-207">adversary</span></span>|<span data-ttu-id="f798d-208">O indicador descreve o adversário.</span><span class="sxs-lookup"><span data-stu-id="f798d-208">The indicator describes the adversary.</span></span>|
|<span data-ttu-id="f798d-209">função</span><span class="sxs-lookup"><span data-stu-id="f798d-209">capability</span></span>|<span data-ttu-id="f798d-210">O indicador é uma capacidade do adversário.</span><span class="sxs-lookup"><span data-stu-id="f798d-210">The indicator is a capability of the adversary.</span></span>|
|<span data-ttu-id="f798d-211">ti</span><span class="sxs-lookup"><span data-stu-id="f798d-211">infrastructure</span></span>|<span data-ttu-id="f798d-212">O indicador descreve a infraestrutura do adversário.</span><span class="sxs-lookup"><span data-stu-id="f798d-212">The indicator describes infrastructure of the adversary.</span></span>|
|<span data-ttu-id="f798d-213">vítima</span><span class="sxs-lookup"><span data-stu-id="f798d-213">victim</span></span>|<span data-ttu-id="f798d-214">O indicador descreve a vítima do adversário.</span><span class="sxs-lookup"><span data-stu-id="f798d-214">The indicator describes the victim of the adversary.</span></span>|

### <a name="killchain-values"></a><span data-ttu-id="f798d-215">valores de killChain</span><span class="sxs-lookup"><span data-stu-id="f798d-215">killChain values</span></span>

| <span data-ttu-id="f798d-216">Valores</span><span class="sxs-lookup"><span data-stu-id="f798d-216">Values</span></span> | <span data-ttu-id="f798d-217">Descrição</span><span class="sxs-lookup"><span data-stu-id="f798d-217">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="f798d-218">Ações</span><span class="sxs-lookup"><span data-stu-id="f798d-218">Actions</span></span>|<span data-ttu-id="f798d-219">Representa "ações nos objetivos".</span><span class="sxs-lookup"><span data-stu-id="f798d-219">Represents “Actions on Objectives”.</span></span> <span data-ttu-id="f798d-220">O invasor está aproveitando o sistema comprometido para realizar ações como um ataque de negação de serviço distribuído.</span><span class="sxs-lookup"><span data-stu-id="f798d-220">The attacker is leveraging the compromised system to take actions such as a distributed denial of service attack.</span></span>|
|<span data-ttu-id="f798d-221">C2</span><span class="sxs-lookup"><span data-stu-id="f798d-221">C2</span></span>|<span data-ttu-id="f798d-222">Representa o canal de controle pelo qual um sistema comprometido é manipulado.</span><span class="sxs-lookup"><span data-stu-id="f798d-222">Represents the control channel by which a compromised system is manipulated.</span></span>|
|<span data-ttu-id="f798d-223">Entrega</span><span class="sxs-lookup"><span data-stu-id="f798d-223">Delivery</span></span>|<span data-ttu-id="f798d-224">O processo de distribuição do código de exploração para vítimas (por exemplo, USB, email, sites).</span><span class="sxs-lookup"><span data-stu-id="f798d-224">The process of distributing the exploit code to victims (for example USB, email, websites).</span></span>|
|<span data-ttu-id="f798d-225">Invasão</span><span class="sxs-lookup"><span data-stu-id="f798d-225">Exploitation</span></span>|<span data-ttu-id="f798d-226">O código de exploração que aproveita as vulnerabilidades (por exemplo, execução de código).</span><span class="sxs-lookup"><span data-stu-id="f798d-226">The exploit code taking advantage of vulnerabilities (for example, code execution).</span></span>|
|<span data-ttu-id="f798d-227">Instalação</span><span class="sxs-lookup"><span data-stu-id="f798d-227">Installation</span></span>|<span data-ttu-id="f798d-228">Instalação de malware após uma vulnerabilidade ter sido explorada.</span><span class="sxs-lookup"><span data-stu-id="f798d-228">Installing malware after a vulnerability has been exploited.</span></span>|
|<span data-ttu-id="f798d-229">Reconhecimento</span><span class="sxs-lookup"><span data-stu-id="f798d-229">Reconnaissance</span></span>|<span data-ttu-id="f798d-230">O indicador é uma evidência de um grupo de atividades que coleta informações a serem usadas em um ataque futuro.</span><span class="sxs-lookup"><span data-stu-id="f798d-230">Indicator is evidence of an activity group harvesting information to be used in a future attack.</span></span>|
|<span data-ttu-id="f798d-231">Armas</span><span class="sxs-lookup"><span data-stu-id="f798d-231">Weaponization</span></span>|<span data-ttu-id="f798d-232">Transformar uma vulnerabilidade em código de exploração (por exemplo, malware).</span><span class="sxs-lookup"><span data-stu-id="f798d-232">Turning a vulnerability into exploit code (for example, malware).</span></span>|

### <a name="tlplevel-values"></a><span data-ttu-id="f798d-233">valores de tlpLevel</span><span class="sxs-lookup"><span data-stu-id="f798d-233">tlpLevel values</span></span>

<span data-ttu-id="f798d-234">Todos os indicadores devem ter um valor de protocolo de semáforo (TLP) quando ele é enviado.</span><span class="sxs-lookup"><span data-stu-id="f798d-234">Every indicator must have a Traffic Light Protocol (tlp) value when it is submitted.</span></span> <span data-ttu-id="f798d-235">Esse valor representa a sensibilidade e o escopo de compartilhamento de um determinado indicador.</span><span class="sxs-lookup"><span data-stu-id="f798d-235">This value represents the sensitivity and sharing scope of a given indicator.</span></span>

| <span data-ttu-id="f798d-236">Valores</span><span class="sxs-lookup"><span data-stu-id="f798d-236">Values</span></span> | <span data-ttu-id="f798d-237">Descrição</span><span class="sxs-lookup"><span data-stu-id="f798d-237">Description</span></span> |
|:-------|:------------|
|<span data-ttu-id="f798d-238">Branco</span><span class="sxs-lookup"><span data-stu-id="f798d-238">White</span></span>| <span data-ttu-id="f798d-239">Escopo de compartilhamento: ilimitado.</span><span class="sxs-lookup"><span data-stu-id="f798d-239">Sharing scope: Unlimited.</span></span> <span data-ttu-id="f798d-240">Os indicadores podem ser compartilhados livremente, sem restrição.</span><span class="sxs-lookup"><span data-stu-id="f798d-240">Indicators can be shared freely, without restriction.</span></span>|
|<span data-ttu-id="f798d-241">Verde</span><span class="sxs-lookup"><span data-stu-id="f798d-241">Green</span></span>| <span data-ttu-id="f798d-242">Escopo de compartilhamento: Comunidade.</span><span class="sxs-lookup"><span data-stu-id="f798d-242">Sharing scope: Community.</span></span> <span data-ttu-id="f798d-243">Os indicadores podem ser compartilhados com a comunidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="f798d-243">Indicators can be shared with the security community.</span></span>|
|<span data-ttu-id="f798d-244">Âmbar</span><span class="sxs-lookup"><span data-stu-id="f798d-244">Amber</span></span>| <span data-ttu-id="f798d-245">Escopo de compartilhamento: limitado.</span><span class="sxs-lookup"><span data-stu-id="f798d-245">Sharing scope: Limited.</span></span> <span data-ttu-id="f798d-246">Essa é a configuração padrão para indicadores e restringe o compartilhamento apenas àqueles que têm de ser conhecidos: 1) serviços e operadores de serviço que implementam inteligência de ameaças; 2) clientes cujos sistemas apresentam comportamento consistente com o indicador.</span><span class="sxs-lookup"><span data-stu-id="f798d-246">This is the default setting for indicators and restricts sharing to only those with a need-to-know: 1) Services and service operators that implement threat intelligence; 2) Customers whose system(s) exhibit behavior consistent with the indicator.</span></span>|
|<span data-ttu-id="f798d-247">Vermelho</span><span class="sxs-lookup"><span data-stu-id="f798d-247">Red</span></span>| <span data-ttu-id="f798d-248">Escopo de compartilhamento: pessoal.</span><span class="sxs-lookup"><span data-stu-id="f798d-248">Sharing scope: Personal.</span></span> <span data-ttu-id="f798d-249">Esses indicadores devem ser compartilhados apenas diretamente e, preferencialmente, em pessoa.</span><span class="sxs-lookup"><span data-stu-id="f798d-249">These indicators are to only be shared directly and, preferably, in person.</span></span> <span data-ttu-id="f798d-250">Normalmente, os indicadores vermelhos do TLP não são incluídos devido às restrições predefinidas.</span><span class="sxs-lookup"><span data-stu-id="f798d-250">Typically, TLP Red indicators are not ingested due to their pre-defined restrictions.</span></span> <span data-ttu-id="f798d-251">Se TLP indicadores vermelhos forem enviados, a propriedade **passiveOnly** também deverá ser definida `True` como.</span><span class="sxs-lookup"><span data-stu-id="f798d-251">If TLP Red indicators are submitted, the **passiveOnly** property should be set to `True` as well.</span></span> |

## <a name="response"></a><span data-ttu-id="f798d-252">Resposta</span><span class="sxs-lookup"><span data-stu-id="f798d-252">Response</span></span>

<span data-ttu-id="f798d-253">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f798d-253">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="f798d-254">Se o cabeçalho de solicitação opcional for usado, o método retornará `200 OK` um código de resposta e o objeto [tiIndicator](../resources/tiindicator.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f798d-254">If the optional request header is used, the method returns a `200 OK` response code and the updated [tiIndicator](../resources/tiindicator.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f798d-255">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f798d-255">Examples</span></span>

### <a name="example-1-request-without-prefer-header"></a><span data-ttu-id="f798d-256">Exemplo 1: solicitação sem cabeçalho de preferência</span><span class="sxs-lookup"><span data-stu-id="f798d-256">Example 1: Request without Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="f798d-257">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f798d-257">Request</span></span>

<span data-ttu-id="f798d-258">Veja a seguir um exemplo da solicitação sem `Prefer` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="f798d-258">The following is an example of the request without the `Prefer` header.</span></span>

# <a name="http"></a>[<span data-ttu-id="f798d-259">HTTP</span><span class="sxs-lookup"><span data-stu-id="f798d-259">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f798d-260">C#</span><span class="sxs-lookup"><span data-stu-id="f798d-260">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f798d-261">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f798d-261">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f798d-262">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f798d-262">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f798d-263">Resposta</span><span class="sxs-lookup"><span data-stu-id="f798d-263">Response</span></span>

<span data-ttu-id="f798d-264">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f798d-264">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a><span data-ttu-id="f798d-265">Exemplo 2: solicitação com cabeçalho preferencial</span><span class="sxs-lookup"><span data-stu-id="f798d-265">Example 2: Request with Prefer header</span></span>

#### <a name="request"></a><span data-ttu-id="f798d-266">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f798d-266">Request</span></span>

<span data-ttu-id="f798d-267">Veja a seguir um exemplo da solicitação que inclui o `Prefer` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="f798d-267">The following is an example of the request that includes the `Prefer` header.</span></span>

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

#### <a name="response"></a><span data-ttu-id="f798d-268">Resposta</span><span class="sxs-lookup"><span data-stu-id="f798d-268">Response</span></span>

<span data-ttu-id="f798d-269">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f798d-269">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="f798d-270">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f798d-270">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f798d-271">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f798d-271">All the properties will be returned from an actual call.</span></span>

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
