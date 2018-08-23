# <a name="deviceenrollmentfailurereason-enum-type"></a>tipo enumerado deviceEnrollmentFailureReason

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em versão prévia e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Principais categorias de falha para inscrição.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|Valor padrão, o motivo da falha é desconhecido.|
|authentication|1|Falha na autenticação|
|authorization|2|Chamada foi autenticada, mas não autorizada a registrar.|
|accountValidation|3|Falha ao validar a conta para o registro. (Conta bloqueada, registro não habilitado)|
|userValidation|4|Usuário não pôde ser validado. (Usuário não existe, não tem licença)|
|deviceNotSupported|5|Gerenciamento de dispositivos móveis não oferece suporte ao dispositivo.|
|inMaintenance|6|Conta está em manutenção.|
|badRequest|7|Cliente enviou uma solicitação que não é compreendida/suportada pelo serviço.|
|featureNotSupported|8|Os recursos usados por esta inscrição não são suportados para essa conta.|
|enrollmentRestrictionsEnforced|9|Restrições de inscrição configuradas pelo administrador bloquearam essa inscrição.|
|clientDisconnected|10|Tempo esgotado ou a inscrição foi abortada pelo usuário final.|



