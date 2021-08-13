---
title: Tipo de número remoteAssistanceOnboardingStatus
description: O status atual do conector teamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 04e9c73c0b0e1c6218332169bea16e3ccc2900772745008525ab1b2b031de7b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182431"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>Tipo de número remoteAssistanceOnboardingStatus

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O status atual do conector teamViewer

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notOnboarded|0|O status relatado quando não há um conector TeamViewer ativo configurado ou ativo|
|integração|1|O status relatado quando o sistema iniciou uma conexão TeamViewer, mas o serviço ainda não concluiu a confirmação de um conector|
|onboarded|2|O status relatado quando o sistema troca com êxito informações de conta com o TeamViewer e agora pode iniciar sessões de assistência remota com clientes|




