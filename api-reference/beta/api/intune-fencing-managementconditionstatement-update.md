---
title: Atualizar managementConditionStatement
description: Atualize as propriedades de um objeto managementConditionStatement.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 33bee3fe6e386d9d426eb0763ccb608cbc6242e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829446"
---
# <a name="update-managementconditionstatement"></a>Atualizar managementConditionStatement

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualize as propriedades de um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria o [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo para a declaração de condição de gerenciamento. Valor atribuído quando criado gerado pelo sistema.|
|displayName|Cadeia de caracteres|O nome definido admin da declaração de condição de gerenciamento.|
|description|Cadeia de caracteres|O administrador definidos descrição da declaração de condição de gerenciamento.|
|createdDateTime|DateTimeOffset|A hora em que a declaração de condição de gerenciamento foi criada. Lado de serviço gerado.|
|modifiedDateTime|DateTimeOffset|A hora que da última modificação a declaração de condição de gerenciamento. Lado de serviços atualizado.|
|expressão|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|A expressão da instrução gerenciamento condição usada para avaliar se um gerenciamento de condição instrução foi ativado/desativado.|
|eTag|String|ETag da declaração de condição de gerenciamento. Lado de serviços atualizado.|
|applicablePlatforms|coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|As plataformas aplicáveis para esta declaração de condição de gerenciamento.
Isso é calculado a partir procurando as condições de gerenciamento associadas ao gerenciamento de condição de instrução e encontrar a interseção de plataformas aplicáveis. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
Content-type: application/json
Content-length: 256

{
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```





